# 常用命令

### 提交
+ 暂存 `git add <file>`
+ 当前状态 `git status`
+ 取消暂存 `git reset HEAD <file>`
+ 提交 `git commit -m ""`
+ 查看修改内容 `git diff <file>`
+ `git push`

### 版本回退
+ 日志记录 `git log --pretty=oneline`
+ 命令记录 `git reflog`
+ `git reset --hard <id>`
  - HEAD表示当前版本，上一个版本就是HEAD^，HEAD^^, HEAD~100
  - --hard 

### 分支命令
+ 查看分支  `git branch -a`
+ 创建分支  `git branch <name>`
+ 切换分支  `git checkout <name>`
+ 创建+切换分支 `git checkout -b <name>`
+ 删除分支 `git branch -d <name>`
+ 发布分支到远程 `git push origin <name>`
+ 删除远程分支 `git push origin --delete <name>`
+ 合并某分支到当前分支：`git merge <name>`