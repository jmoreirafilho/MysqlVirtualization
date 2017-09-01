Vagrant.configure("2") do |config|
    config.vm.box = "ubuntu/xenial64"
    config.vm.network :forwarded_port, guest: 80, host: 8080
	config.vm.network :forwarded_port, guest: 3306, host: 3306
    config.vm.synced_folder "./vagrant", "/vagrant", :mount_options => ["dmode=777","fmode=666"]
    config.vm.provider "virtualbox" do |machine|
    	machine.memory = 1024
    	machine.name = "ubuntu-server-mysql"
    end
    config.vm.provision :shell, path: "setup.sh"
end
