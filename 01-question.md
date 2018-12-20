# 常见问题
+ 提交代码有冲突
+ 拉取代码有冲突
+ 代码已commit，发现有问题，需要回退
+ 回退后悔
+ 代码已push，发现有问题，需要回滚
+ 切换分支有冲突
+ 合并代码有冲突

# 问题提示
+ 提交代码有冲突
  ```
   error: failed to push some refs to 'https://github.com/XXX/xxx.git'
   hint: Updates were rejected because the tip of your current branch is behind
   hint: 'git pull ...') before pushing again.
  ```

+ 拉取代码有冲突
  ```
  error: Your local changes to the following files would be overwritten by merge:
        readme.md
  Please commit your changes or stash them before you merge.
  ```
    
+ 代码已commit，发现有问题，需要回退

+ 回退后悔了

+ 代码已push，发现有问题，需要回滚

+ 切换分支有冲突 `git checkout <branchName>` 

  ![](images/checkout-branch.jpg)

+ 合并代码有冲突 `git merge <branchName>`
  ```
  CONFLICT (content): Merge conflict in develop.md
  Automatic merge failed; fix conflicts and then commit the result.
  ```

