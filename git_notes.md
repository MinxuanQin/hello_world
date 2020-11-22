### vscode快捷键
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


Caution:
1. commit 指记录当前工作树所有文件的**当前**状态
