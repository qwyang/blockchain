# 2018/12/05:install ethereum development invironment.
## install virtualbox on windows
## dowload ubuntu16.04 ISO
## install ubuntu virtual machine
## install virtualbox enhancement package for vm
## 实现host和vm之间复制粘贴功能，虚拟机启动后，设备->拖放->双向
## 安装git工具，github新建blcokchain仓库
	git init
	git add README.md
	git commit -m "first commit"
	git remote add origin git@github.com:qwyang/blockchain.git
	git push -u origin master
## 虚拟机安装golang
## 虚拟机安装geth客户端
	sudo apt-get install software-properties-common
	sudo add-apt-repository -y ppa:ethereum/ethereum
	sudo apt-get update
	sudo apt-get install ethereum
## 安装nodejs
	curl -sL https://deb.nodesource.com/setup_10.x | sudo -E bash -
	sudo apt-get install -y nodejs
	dpkg -L nodejs | grep /usr/bin
	sudo npm install n -g
## 虚拟机安装remix-ide编译器
	git clone https://github.com/ethereum/remix-ide.git
	cd remix-ide
	npm install
	npm start
