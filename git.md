# git

## 修改相关配置

git config --list  # 显示配置

git config --global user.name  # lk 配置用户名

git config --global user.email xxxx.@xx.com  # 配置邮箱

git config --global core.editor "'D:\Sublime Text\subl.exe' -w"  # 配置默认文本编辑器

git config --global --unset 配置名称  # 删除相关配置

## add & commit

创建新文件（或做修改）之后，先 git add xxx.xx 添加文件（提交到缓存）；然后 git commit xxx.xx [-m (添加注释)] 提交文件（提交到本地仓库，默认提交到master分支）。

## 查看仓库状态： git status [-s]

## 查看修改历史： git log [xx.xx(指定文件), --oneline(一行显示)]

## 比较差异： git diff

## 还原修改 ：

## 删除文件： git rm xxx.xx

# 连接远端仓库

## 生成ssh密钥： 

ssh-keygen -t rsa；在GitHub中的SSH设置中将公钥复制过去

## 为远程仓库起别名(方便输入)：

git remote add 别名 远程仓库地址

git remote add origin git@github.com:Karity/git.git（将git@github.com:Karity/git.git命名为origin(在git config -l中可看到，即：remote.origin.url=git@github.com:Karity/git.git，也可在.git目录下的config文件中查看字段：[remote "xxx"] url=xxx)，

git@github.com:Karity/git.git这个名称是在GitHub中创建的仓库的git地址）

## 推送到远程仓库：

git push -u origin master

## 查看及删除远程仓库：

git remote -v  # 查看关联的远端仓库(即起的别名)，也可在.git目录下的config文件中查看字段：[remote "xxx"] url=xxx

git remote rm 仓库名  # 删除仓库

## 创建分支

git branch 分支名

## 切换分支

git checkout 分支名