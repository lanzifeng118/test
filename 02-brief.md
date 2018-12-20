# 简介
### 分布式版本控制系统
  - 安装
  - 配置 `git config`

### 四个工作区域
+ 工作区
  - 平时存放项目代码的地方

+ 版本库
  - 克隆资源 `git clone <资源>` 
  - 初始化 `git init` 
  - .git目录 HEAD、refs、index、logs

+ 暂存区
  - .git/index
  - 用于临时存放改动，事实上它只是一个文件，保存即将提交到文件列表信息

+ 远程仓库
  - github、gitlab
  
  <img src="images/git.jpg" width="600" style="display: block;"/> 

### 文件的四种状态 `git status`
  + untracked 未跟踪, 此文件在文件夹中, 但并没有加入到git库, 即新建文件
  + unmodified 文件已经入库, 未修改
  + modified: 文件已修改, 仅仅是修改, 并没有进行其他的操作
  + staged: 暂存状态
  <img src="images/status.png" width="600"/>

### git工具 储藏Stashing
  + 开发到一半,同步远端代码、工作流被打断,需要先做别的需求
  + 获取你工作目录的中间状态，并将它保存到一个未完结变更的堆栈中，随时可以重新应用
  + 查看 `git stash list`
  + 储藏 `git stash`
  + 应用 `git stash apply <name>` 或者 `git stash pop`
  + 删除 `git stash drop <name>`
  + 查看diff `git stash show -p <name>`
  + 创建分支 `git stash branch <branchName>`

### 分支管理
#### 工作流：支管理策略，仅是一个规则，完全由开发者自定义，并且自遵守

  + git flow
    - 两个长期分支: 主分支master, 开发分支develop
    - 功能分支 补丁分支 预发分支
    <img src="images/workflow-git.png" width="600" style="display: block;"/> 
    - 缺点：相对复杂，需要同时维护两个长期分支。很多项目是"持续发布"，代码有变动，就部署一次。这时，master分支和develop分支的差别不大

  + github flow
    - 简单版git flow，只有一个长期分支，就是master
    <img src="images/github_flow.png" width="200" style="display: block;"/>  
    <img src="images/workflow-github.png" width="600" style="display: block;"/>  

    - 缺点：master分支与发布的版本不一致、不同环境、不同版本

  + gitlab flow
    - 最大原则叫做"上游优先"，只存在一个主分支master，它是所有其他分支的"上游"。只有上游分支采纳的代码变化，才能应用到其他分支。
    - 持续发布
    <img src="images/environment_branches.png" width="300" style="display: block;"/>  

    - 版本控制 
    <img src="images/release_branches.png" width="300" style="display: block;"/>  
  + 查看分支：`git branch -a`
  + 创建分支：`git branch <name>`
  + 切换分支：`git checkout <name>`
  + 创建+切换分支：`git checkout -b <name>`
  + 合并某分支到当前分支：`git merge <name>`
  + 删除分支：`git branch -d <name>`
  + 删除远程分支 `git push origin --delete <name>`