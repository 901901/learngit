添加文件：git add 文件名； git commit -m "文件描述"；
查看工作区状态: git status；
查看修改内容：git diff；
查看历史记录：git log；git log --pretty=oneline；
回退以前版本：HEAD是指向当前版本的指针、回退时是改变HEAD指向
未关闭当前窗口
git reset --hard HEAD^(HEAD^^回退两次、HEAD~100回退一百次)；
git reset --hard "commit id"；
已关闭当前窗口，重新打开查看以前记录：git reflog

查看.git目录：.git目录是跟踪管理版本库

git is a distributed version control system.
git is free software distributed under the GPL.
say something
