# Linuxmint下配Git
## 一.安装git软件
 sudo apt-get install git 
## 二.配置本地SSH KEY
ssh-keygen -t rsa -C "xxx@gmail.com"
## 三.将SSH KEY拷贝到GitHub网站
将.ssh/id_rsa.pub拷贝到GitHub网站
## 四.测试SSH KEY 是否成功
$ssh -T git@github.com
如果出现You've successfully authenticated, but GitHub does not provide shell access.
则表示成功。
## 五. 配置Git的配置文件
git config --global user.name "your name" //配置用户名
git config --global user.email "your email" //配置email 
##六.克隆目录，操作git
$cd ~
$mkdir GithubPro
$cd GithubPro
$mkdir notes
使用命令 "git clone https://github.com/beautyofsoul/notes.git"