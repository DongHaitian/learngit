$ mkdir 文件夹名称
$ cd 文件夹名称
$ pwd
: 生成文件夹并显示当前目录
$ git init
: 使该目录编程Git可以管理的仓库
$ git add 文本名称.文本格式
：将文件添加到仓库
$ git commit -m "文件备注"
:  将文件提交到仓库
注：”git add 可以反复使用添加多个文件
$ git status 
: 可以看到当前时刻仓库状态
$ git diff 文本名称.文本格式
: 查看文本修改
$ git log
: 可查看该文本提交日期
$ git reset --hard HEAD^
：将文本返回到上一版本，上两个为HEAD^^，过多时可用HEAD~x
$ cat 文本名称.文本格式
：可看见文本当前版本内容
$ git reset --hard 版本号
：可指定回到未来的某个版本（版本号不一定要写全，git会自己搜索）
$ git reflog
: 记录我的每一次命令
注：git log可查看提交历史，以便回退到哪个版本，git reflog 以便回到未来的哪个版本
$ git checkout -- readme.txt
: 丢弃工作区的修改
$ git reset HEAD <file>
: 把暂存区的修改撤销掉
$ git rm test.txt
$ git commit -m "remove test.txt"
: 从版本库中删除该文件
$ git checkout -- test.txt
: 还原（需曾提交到版本库过）
查看分支：git branch

创建分支：git branch <name>

切换分支：git checkout <name>或者git switch <name>

创建+切换分支：git checkout -b <name>或者git switch -c <name>

合并某分支到当前分支：git merge <name>

删除分支：git branch -d <name>
 git stash  储藏区
 git stash list  储藏区名单
git stash apply恢复，但是恢复后，stash内容并不删除，你需要用git stash drop来删除；
git stash pop，恢复的同时把stash内容也删了：
 git stash apply stash@{0}  恢复指定的stash
$ git cherry-pick 复制一个特定的提交到当前分支
$ git branch -D 强行删除
$ git remote add origin {remote_repo_addr}




. 当前目录
.. 上一级目录
~ home目录
/ 根目录



