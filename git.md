# 连接远端仓库

## 生成ssh密钥： 

https://blog.csdn.net/weixin_47082552/article/details/125963913

ssh-keygen -t rsa (按三次回车)；将生成的id_rsa.pub 复制到GitHub中的SSH设置 ->SSH and GPG keys -> 新建ssh

## 为远程仓库起别名(方便输入)：

git remote add 别名 远程仓库地址

git remote add origin git@github.com:Karity/git.git（将git@github.com:Karity/git.git命名为origin(在git config -l中可看到，即：remote.origin.url=git@github.com:Karity/git.git，也可在.git目录下的config文件中查看字段：[remote "xxx"] url=xxx)，

git@github.com:Karity/git.git这个名称是在GitHub中创建的仓库的git地址）

## 推送到远程仓库：

git push -u origin master

## 查看及删除远程仓库：

git remote -v  # 查看关联的远端仓库(即起的别名)，也可在.git目录下的config文件中查看字段：[remote "xxx"] url=xxx

git remote rm 仓库名  # 删除仓库

## 查看所有分支

[Git从入门到精通(下篇)-5-分支详解 - 知乎 (zhihu.com)](https://zhuanlan.zhihu.com/p/410255613#:~:text=git branch可以查看当前所有的分支%2C,本质上是显示.git%2Frefs%2Fheads 目录下的文件.)

git branch

## 创建分支

git branch 分支名

## 切换分支

git checkout 分支名

# git

## 1.git init 初始化仓库

## 修改相关配置

git config --list  # 显示配置

git config --global user.name  # lk 配置用户名

git config --global user.email xxxx.@xx.com  # 配置邮箱

git config --global core.editor "'D:\Sublime Text\subl.exe' -w"  # 配置默认文本编辑器

git config --global --unset 配置名称  # 删除相关配置

## 2.add & commit

创建新文件（或做修改）之后，先 git add xxx.xx 添加文件（提交到缓存）；然后 git commit xxx.xx [-m (添加注释)] 提交文件（提交到本地仓库，默认提交到master分支）。

`git add -A .` 来一次添加所有改变的文件；`git add .` 表示添加新文件和编辑过的文件不包括删除的文件； `git add -u` 表示添加编辑或者删除的文件，不包括新添加的文件

## 3.推送到远程仓库：

git push -u origin master

## 查看仓库状态： git status [-s]

## 查看修改历史： git log [xx.xx(指定文件), --oneline(一行显示)]

## 比较差异： git diff

## 还原修改 ：

## 删除文件： git rm xxx.xx

