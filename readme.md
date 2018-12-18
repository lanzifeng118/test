# 文档

### 提交
+ `git add`
+ `git commit -m ""`
+ 当前状态 `git status`
+ 查看修改内容 `git diff <file>`
+ `git push`

### 版本回退
+ `git log --pretty=oneline`
+ `git reset --hard <id>`
  - HEAD表示当前版本，上一个版本就是HEAD^，HEAD^^, HEAD~100
  - --hard 
+ 记录每次命令 `git reflog`

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

## 常遇问题
+ 提交代码有冲突
  ```
   An error occurred while sending the request.
   ! rejected release-readme -> release-readme (non-fast-forward)
   error: failed to push some refs to 'https://github.com/XXX/test.git'
   hint: Updates were rejected because the tip of your current branch is behind
  ```
+ 拉取代码有冲突
  ```
  error: Pulling is not possible because you have unmerged files.
  hint: Fix them up in the work tree, and then use 'git add/rm <file>'
  hint: as appropriate to mark resolution and make a commit.
  fatal: Exiting because of an unresolved conflict.
  ```
  ```
  error: Your local changes to the following files would be overwritten by merge:
        readme.md
  Please commit your changes or stash them before you merge.
  ```
+ 
https://www.liaoxuefeng.com/wiki/0013739516305929606dd18361248578c67b8067c8c017b000/001374831943254ee90db11b13d4ba9a73b9047f4fb968d000

****