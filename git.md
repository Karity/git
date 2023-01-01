# git

## 修改相关配置

### git config --list 显示配置

### git config --global user.name lk 配置用户名

### git config --global user.email xxxx.@xx.com 配置邮箱

### git config --global core.editor "'D:\Sublime Text\subl.exe' -w" 配置默认文本编辑器

## add commit

### 创建新文件（或做修改）之后，先 git add xxx.xx 添加文件（提交到缓存）；然后 git commit xxx.xx [-m (添加注释)] 提交文件（提交到本地仓库，默认提交到master分支）。

## 查看仓库状态： git status [-s]

## 查看修改历史： git log [xx.xx(指定文件), --oneline(一行显示)]

## 比较差异： git diff

## 还原修改 ：

## 删除： git rm xxx.xx