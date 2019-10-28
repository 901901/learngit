添加文件：
	git add fileName:把文件添加进去-把文件修改添加到stage暂存区；
	git commit -m "fileDescription":提交更改-把暂存区所有的内容提交到当前分支；

查看工作区状态:
	git status；

查看修改内容：
	git diff；

查看历史记录：
	git log；git log --pretty=oneline；

回退以前版本：HEAD是指向当前分支该版本的指针、回退时是改变HEAD指向
未关闭当前窗口
	git reset --hard HEAD^(HEAD^^回退两次、HEAD~100回退一百次)；
	git reset --hard commitId；
	已关闭当前窗口，重新打开查看以前记录：git reflog

查看.git目录：
	.git目录是跟踪管理版本库

撤销操作：如果提交到了版本库则可以恢复文件到最新版本、丢失最近一次修改的内容
	丢弃工作区的修改、回到最近一次git commit或者git add状态
	git checkout --fileName 
	把暂存区的修改回退到工作区：git reset HEAD fileName
	
删除文件：
	rm fileName：然后git rm fileName、git commit-m"descripition"；

关联远程库：
	git remote add origin git@901901：path/repo-name.git
	关联后第一次推送master分支的所有内容：git push -u origin master
	此后每次本地提交后推送最新修改：git push origin master

从远程库克隆：
	git clone git@github.com:githubName/repositoryName.git
	
say something