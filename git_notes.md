### vscode快捷键
快捷键链接：<https://segmentfault.com/a/1190000012811886>
1. 向上的箭头表示shift键
2. 打开command：`command + shift + p`
3. 打开preview（侧边）：`command + k, + v`

### git指令
|指令|说明|
|---|---|
|git init|初始化仓库，`.git`管理仓库数据|
|git status|查看状态|
|git add|将文件加入暂存区中(Stage/index)|
|git commit -m "..."|记述一行提交信息|
|git  commit|启动编辑器，记述详细提交信息<br>`#`内容可忽略，第一行为简述<br>第二行为空行，三行以后记录详细内容|
|git log<br>--pretty=short<br>filename<br>-p|查看提交日志，commit后的数字串为哈希值<br>只显示简略信息<br>只显示文件/目录相关<br>显示改动|
|git log --graph|以图表形式输出提交日志|
|git diff<br>git diff HEAD|比较工作树和暂存区差别|
|git branch|显示分支一览表，当前分支前有`*`|
|git checkout -b|以当前分支为基础创建新分支|
|git checkout 'brach_name'|切换分支|
|git checkout -|切换到上一分支|
|git merge --no-ff 'branch_name'|合并分支，自动打开编辑器添加commit备注|

**Caution:**
1. commit 指记录当前工作树所有文件的**当前**状态
2. 在`git commit`之前先执行一次`git diff HEAD`,HEAD指向当前分支中最新一次提交的指针
3. `git branch feature-A` 和 `git checkout feature-A`可以取得一样的效果：创建新分支
4. 不断对一个分支进行提交的操作叫“培育分支”
5. 基于特定主题的作业在特定分支中进行，完成之后再与master分支合并。这样可以保证**master分支可以随时供人查看**。
6. 在合并分支前需要将当前分支所有变化提交(commit)