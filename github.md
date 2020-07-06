## github

## Github建立组织团队

01. 使用Github网上大多数是采用ssh连接，需要输入密钥。Github desktop可以简单的解决这一问题
02. 主机人员添加New Organization输入组织名，接收邮箱等
03. 添加组织人员也就是不同账号，不用理会下一页的体验改进调查
04. 创建一个新的项目同时可以也邀请团队人员，被邀请者查看邮箱确认join（注：Team应在Organization里）
05. 创建团队：
06. 权限只能给某团队唯一权限（管理员、只写、只读）进入到code标签页---》settings---》collaboration---》Team进行权限控制（第一次需输入密码）
07. 删除在settings，但是要输入需删除的名称，以免误删

## Github使用桌面版

08. 下载Github桌面版
09. 打开软件使用注册或者已有的邮箱密码进行登录，选择File-》Clone repository 同步github上的文件并确定保存本地地址路径
10. 用编辑器修改操作文件，和源文件相比如有改动则会显示在github桌面版左上角列表，而后在左下角输入摘要后，先保存在自己的本地中，选择push 推到github上
11. 自己本地和github同步则用pull拉
12. 若多个账户同时操作同一个文件，一个账户提交后，先commit到本地，然后pull一下，此时会出现两种状况：（1）同一个文件同一个地方更改时：弹窗报错并在文件中显示出来不同之处【标注】（2）同一个文件不同地方更改时：覆盖后以最后提交者为准
13. 提交文件的步骤：先把更改的文件保存在本地---》pull---》push
14. 多个账户一起协作一般都会建立多个分支来完成不同功能
15. 分支和主线的区别在于不破坏主线内容的同时进行修改等
16. 由支线更新到主线（合并分支）：切换到主线---》Branch---》Merge---》选择支线
17. 由主线更新到支线：切换到支线---》update

## 通过命令如何使用

commit 之后：
git fetch origin master:temp 创建个临时分支
git  stash  有其他没有必须提交的文件执行，也就是暂存一下
git  pull --rebase
git rebase temp
git push 
git branch -D temp 删除临时分支
git stash pop

提交临时版：
git cherry-pick 自己的提交时候生成的号
git pull --rebase
git push

其他命令：
git status查看下
git branch 有那几个分支

