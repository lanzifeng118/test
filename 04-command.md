# 常用命令
### 初始化项目
+ `git init` 初始化
+ `git clone <url>` 克隆

### 基本操作
+ `git add <file>` 暂存
+ `git reset HEAD <file>` 取消暂存
+ `git commit -m ""` 提交本地
+ `git reset <id>` 撤销本地修改
+ `git push` 提交远程
+ `git revert <id>` 回退
+ `git pull` 拉取

### 查看
+ `git status` 当前状态
+ `git diff <file>` 查看修改内容
+ `git log --pretty=oneline` 日志记录
+ `git reflog` 命令记录

### 分支命令
+ `git branch -a` 查看分支  
+ `git branch <name>` 创建分支  
+ `git checkout <name>` 切换分支
+ `git checkout -b <name>` 创建+切换分支 
+ `git branch -d <name>` 删除分支 
+ `git push origin <name>` 发布分支到远程 
+ `git push origin --delete <name>` 删除远程分支 
+ `git merge <name>` 合并某分支到当前分支

### 储藏
+ `git stash list` 查看 
+ `git stash` 储藏 
+ `git stash apply <name>` 应用 
+ `git stash pop` 应用 
+ `git stash drop <name>` 删除
+ `git stash show -p <name>` 查看diff
+ `git stash branch <branchName>` 创建分支