# 文档

### 提交
+ 暂存 `git add <file>`

  ![](images/add.png)

+ 当前状态 `git status`
+ 取消暂存 `git reset HEAD <file>`
+ 提交 `git commit -m ""`

  ![](images/commit.png) 
  
+ 查看修改内容 `git diff <file>`
+ `git push`

### 版本回退
+ 日志记录 `git log --pretty=oneline`
+ 命令记录 `git reflog`
+ `git reset --hard <id>`
  - HEAD表示当前版本，上一个版本就是HEAD^，HEAD^^, HEAD~100
  - --hard 

### 工作区和暂存区
+ 暂存区 `.git/index`

### 分支命令
+ 查看分支  `git branch -a`
+ 创建分支  `git branch <name>`
+ 切换分支  `git checkout <name>`
+ 创建+切换分支 `git checkout -b <name>`
+ 删除分支 `git branch -d <name>`
+ 发布分支到远程 `git push origin <name>`
+ 删除远程分支 `git push origin --delete <name>`
***

https://www.liaoxuefeng.com/wiki/0013739516305929606dd18361248578c67b8067c8c017b000/001374831943254ee90db11b13d4ba9a73b9047f4fb968d000
