# Git 的基本操作

## 参考廖雪峰的网站和饥人谷的课程

基本操作

- git add .
- git commit -m "注释"
- git status 查看状态
- git diff 查看不同
- git log 查看历史记录
- git reset --head 回退版本 用 commit id
- git reflog 查看命令历史 回到未来哪个版本
- git add 是将修改从工作区提交到版本库里的暂存区，commit 是将修改提交到 master 也就是当前分支
- git checkout --test.txt 把 test.txt 文件在工作区的修改全部撤销
- git reset HEAD <file> 可以回退版本，也可以把暂存区的修改回退到工作区，用 staus 查看
- rm 删除文件 git status 可以看出变化 git rm 后 git commit 在版本库也删除
- 删除工作区的内容可以通过 git checkout --<file> 使用版本库还原
- 添加远程库 先把 ssh 密匙弄好 创建新仓库 粘贴所提示的 git remote add origin git@.....
- 然后第一次上传 git push -u origin master 之后使用 git push 就可以了
- git remote -v 查看远程库信息 删除分支 git remote rm origin 并不是物理删除远程库，而是解除了本地和远程的绑定关系，删除还是需要登录 github 删除
- git 在对应文件中运行 git clone 加 代码 github 的 ssh 链接
