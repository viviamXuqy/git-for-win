下载git安装包后，一路点点点默认安装
# Window下git生成SSH Key
#### 1.右键鼠标，选中 “Git Bash here”，当然你也可以在windows的 “开始”--->“所以程序”，或者安装目录打开它

#### 2.输入指令，进入.ssh文件夹

> cd ~/.ssh/

#### 如果提示 “ No such file or directory”，你可以手动的创建一个 .ssh文件夹即可
> mkdir ~/.ssh

#### 3.配置全局的name和email，这里是的你github或者bitbucket的name和email

>git config --global user.name "你的用户名" 

>git config --global user.email "你的公司或个人邮箱"

#### 4.生成key
> ssh-keygen -t rsa -C "你的公司或个人邮箱"

连续按三次回车，这里设置的密码就为空了，并且创建了key。

> 最后得到了两个文件：id_rsa和id_rsa.pub

#### 5.打开Admin目录进入.ssh文件夹，用记事本打开id_rsa.pub，复制里面的内容添加到你github或者bitbucket ssh设置里即可
