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

### 文件的四种状态 `git status`
  + untracked 未跟踪, 此文件在文件夹中, 但并没有加入到git库, 即新建文件
  + unmodified 文件已经入库, 未修改
  + modified: 文件已修改, 仅仅是修改, 并没有进行其他的操作
  + staged: 暂存状态
  <img src="images/status.png" width="600"/>