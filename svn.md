####SVN

#####版本管理工具

1. 象模开发时是存在版本的；一个开发之中的时间节点；

####SVN使用

1. 建立线上仓库
2. 在本地 **检出** 线上仓库发送到
3. 右键鼠标点击提交，把本地代码提交到线上仓库。

#####SVN有啥用

1. 防止熊孩子破坏代码

2. 任意版本进行任意切换

####分支 branch

1. 新建分支

> git branch [ 分支名 ] 创建分支
> git branch 查看分支;

2. 切换分支

> git checkout [ 分支名 ]
> 切换并新建分支 git checkout -b [ 分支名 ]

3. 分支中的一切操作和正常的github操作一样;

git add | commit | status | push

4. 合并分支

git merge [ 分支名 ]

#####DOS

1. cd 进入或退出文件夹  .. 表示上一级目录  . 表示当前目录;
2. mkdir 创建文件夹;
3. dir 查看文件夹;
4. 删除文件夹  rd /s /q 文件夹名

##### linux

1. mkdir hello 创建名为hello 的文件夹;
2. pwd 查询当前路径
3. cd 进入|退出文件夹的意思 ..表示上级目录 . 表示当前目录;
4. touch 创建文件夹
5. rm -rf 文件夹名 删除操作  ***高危操作请谨慎执行，一切后果自行承担;
6. ls -a 查看当前文件夹下所有文件(包括隐藏文件夹)

##### git 指令


##### git 初始配置

1. 你要告诉仓库你是谁 : (一台电脑设置一次)

      $ git config [ --global ] iser.name "[ name ]"
      >注册的用户名
      $ git config [ --global ] user.email "[email address]"
      >注册的邮箱地址

2. git 初始化 : (一个项目初始一次)

      $ git init

      >Initialized empty Git repository in
      D:/phpstudy/PHPTutorial/WWW/0121/1823/,git 如果存在表示成功;

3. git 本地索引添加

      $ git add [ name ]
      $ git add -A 添加所有

      > git status 查看状态
      > 如果你添加的文件夹全绿那么表示add没有问题

4. git 工作区放入仓库之中

      $ git commit -m "必须写注释"

##### git 提交操作

add | commit | push

5. 版本还原操作

> 1. 找到对应的版本  查看版本 git refiog
> 2. 根据查看到的版本  进行版本还原 还原指令为 git reset --hard [ 版本号 ]

tip : 只有commit 之后的代码，才有资格还原

6. 给当前的仓库加上一个名为 origin 的源(origin 可以任意改变这就是个变量名)

      git remote add origin
      https://github.com/huaizhiY/1823.git

      tip : 一个仓库设置完了一个源就不用再次重复设置相同的源了;

7. 把本地仓库的内容提交到远程仓库

   git push -u [ 源的名称 ] [ 分支名称 ]

   源的名称 : git remote的时候设置的什么名字就是哪个源;


#！！！警告！！！警告！！！

1. 千万不要把公司开发的项目放在开源仓库里
2. 公司都会有局域网的github => gitlab