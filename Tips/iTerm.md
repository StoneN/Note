- 新建目录 `mkdir <name>`
- 新建文件 `touch xxx.txt`
- 查看文件 `cat xxx.txt`
- 标准输出到文件 `echo "something" > xxx.txt`


# Git
- `git status`
- `git add`
- `git commit -m "desc"`
- `git log --oneline` 以摘要形式查看日志
- `git log --graph` 图形化查看日志
- `git reset --hard/soft <commitId>` 撤销commit
- `git commit --amend` 将修改添加到上次提交
- `git checkout -- <file>` 撤销掉还未 `git add` 的修改
- `git branch <name>` 创建新分支 
- `git branch <name> <被删分支的最后一次commit的id>` 恢复被删除的分支 
- `git branch -m <old name> <new name>` 重命名分支 
- `git checkout <branch name>` 切换分支
- `git checkout -b <branch name>` 创建并切换到新分支
- `git merge <branch name>` 将制定分支合并到当前分支 **[当出现冲突时，需要修改冲突文件，并将修改 `add`+`commit`]**
- `git merge --abort` 放弃合并
- `git rebase <branch name>` 变基，将当前分支接到目标分支的最后一次 commit 之后 **[变基之后到切回指定分支，将该分支 merge]**
- `git branch -d <branch name>` 删除指定分支
- `git stash` 缓存修改
- `git stash list` 查看缓存列表
- `git stash apply <stash@{id}>` 恢复指定 stash 的内容
- `git stash pop <stash@{id}>` 恢复指定 stash，并且删除已恢复的 stash
- `git stash drop <stash@{id}>` 手动删除指定 stash
- `git stash branch <branch name>` 新建分支，并且将指定 stash 内容恢复到该分支

#### Github
- `git remote add origin <github repository url>` 为本地项目添加 GitHub 远程来源
- `git push -u origin master` 将本地项目推送到关联的远程仓库
- `git clone <github repository url> <本地目录>` 将远程库拷贝到本地目录
- `git config credential.helper ""` 清空保存的认证信息
- `git config user.name <xxx>` 设置 Git 的本地名称
- `git config user.email <xxx>` 设置 Github 账号使用的邮箱


