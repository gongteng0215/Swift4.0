# 配置github的ssh密钥: #

1、Windows键+r打开运行，输入cmd
(1)打开Git Bash查看电脑上是否已经存在SSH密钥：
输入 cd ~/.ssh

(2)创建新的ssh key:
输入 ssh-keygen -t rsa -C "your_email@youremail.com" 

执行这条命令会如上图提示文件保存路径，可以直接按Enter，

然后提示输入 passphrase（密码），输入两次（可以不输直接两次Enter），
然后会在 .ssh 目录生产两个文件：id_rsa和id_rsa.pub
用记事本打开.ssh目录下的id_rsa.pub文件，复制里面的内容；
cat ~/.ssh/id_rsa.pub
 
2、复制ssh key到github：
On the GitHub site Click “Account Settings” > Click “SSH Keys” > Click “Add SSH key”

打开github网站，点击右上角扳手图标，然后点击左边菜单的 ssh key， 然后右边页面的 add ssh key，将复制的内容粘贴到github的key中，title可以不填，直接保存即可。


3、测试 ssh 链接 github：
输入 ssh -T git@github.com
出现Successfully就OK；

 

6、设置自己的git信息：
输入
git config --global user.name "Firstname Lastname" （此处name可修改也不是用于登录github的登录名）
git config --global user.email "your_email@youremail.com"
设置自己的git信息即完成安装和设置，可以输入git config --list查看自己的git信息。