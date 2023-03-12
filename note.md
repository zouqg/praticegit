```bash
git init 初始化仓库
git add file 	添加文件到仓库
git commit -m "message" 提交修改
git status 查看当前状态
git diff 查看文件的修改
git reflog 查看git的命令记录
# 每次修改，如果不用git add到暂存区，那就不会加入到commit中
git checkout -- readme.txt 撤销readme.txt在工作区的修改
git reset HEAD readme.txt  撤销readme.txt在暂存区的修改

# 小总结
# 撤销在工作区的修改 git checkout -- file
# 撤销add			 git reset HEAD file ,修改阶段将回到工作区
# 撤销commit		 git reset --hard 版本号

git remote -v 			# 查看远程库信息
git remote rm origin 	# 解除本地库和远程库的连接
git remote add origin git@server-name:path/repo-name.git # 关联一个远程库 origin是默认习惯命名
git push -u origin master 	#第一次推送master分支的所有内容
git push origin master   	# 本地修改后，推送最新修改到远程分支

git 支持两种协议https和ssh(速度快)
	1、 https://github.com/zouqg/praticegit.git
	2、 git@github.com:zouqg/praticegit.git
```

##### 分支管理

> 分支的创建、切换和删除

```bash
 git checkout -b dev  # 创建dev分支并切换到dev分支
 	# 相当于下面两条命令
 	git branch dev
	git checkout dev
git merge dev		# 将dev分支合并到当前分支
git branch -d dev  	# 合并后删除dev分支

# 用switch切换分支
git switch -c dev 	# 创建dev分支并切换
git switch master	# 切换到以后的分支
git branch 			# 创建分支

```

