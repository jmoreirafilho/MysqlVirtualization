# Projeto MySQL Blank #

Servidor (Linux, MySQL)

Máquina vagrant com MySQL instalado e liberado para a máquina host acessar.

### Pacotes Inclusos ###
- MySQL 5.5
(Para mais detalhes consulte arquivo setup.sh)


## Requisitos Mínimos ##

- Virtualbox - https://www.virtualbox.org/
- Vagrant - http://www.vagrantup.com/
- Git - http://git-scm.com ( Opicional )
- Acesso Internet

## Passo a Passo ##

1. Instale o VirtualBox e em seguida o Vagrant


2. Clone o projeto através do comando `git clone http://USER-NAME@git.mdb.com.br/Virtualizacoes/ubuntu-server-mysql.git`
	

3. Dentro da pasta do projeto, pelo Terminal, execute o comando `vagrant up`
	- Esse comando, quando executado pela primeira vez pode demorar mais de uma hora, pois irá:
		* Baixar a VM Ubuntu
		* Instalar o mysql

4. Você poderá acessar o seu banco através de qualquer cliente na máquina host. Seguem dados:
	- Login: **root**
	- Senha: **vagrant**

5. Você poderá acessar a sua máquina através do terminal via ssh, digitando `vagrant ssh` de dentro da pasta do projeto