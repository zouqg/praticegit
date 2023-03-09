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
# 撤销commit		 git reset --hard b
```

