# git ops

## 创建，切换分支

+ `git commit` 在当前分支下创建子节点
+ `git branch nbranch` 创建新的分支 `nbranch`

比起将原来分支修改的冗长复杂，创建新的分支可以逻辑清晰，事半功倍
注意，新版本 `git` 中采用 `switch` 命令实现切换分支的效果 [看这里](https://git-scm.com/docs/git-switch)

+ `git checkout nbranch` 切换到分支`nbranch`
+ `git checkout -b <your-branch-name>` 创建，同时切换到相应分支

## `merge` 操作

+ `git merge nbranch` 将另一个兄弟节点合并到当前所在的 `branch` 上来。
+ 可以通过之前的 `git checkout -b nbranch` 创建并切换到分支上

## `rebase` 操作

`rebase` 也是合并分支的操作，在于取出一系列提交记录，复制之后逐个放到另一个地方。

+ `git rebase main` 将当前指向的分支在main当前分支下创建副本子分支。
+ `git checkout main` 将当前分支指向main
+ `git rebase bugFix` 将main引用切到bugFix上

## 按键绑定
