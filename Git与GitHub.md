# Git与GitHub

### 一、Git命令

```
// 查看git版本
git --version

// 克隆仓库到本地
git clone [仓库地址] 
git clone -o [远程主机名]  [仓库地址]  [本地仓库主目录名]

// 查看本地仓库所关联的远程仓库信息 
git remote -v

// 在仓库主目录查看仓库的状态
git status

// 把新增文件添加到暂存区
git add [文件名]
// 对多个文件或目录进行了增删改，全部添加到暂存区
git add .

// 撤销暂存区的修改
git reset -- [文件名]
// 把暂存区的全部修改撤销
git reset --

// 查看工作区被跟踪的文件的修改详情
git diff
// 查看暂存区的全部修改
git diff --cached

// 查看某分支的提交历史，不写分支名查看当前所在分支
git log [分支名]
// 一行显示提交历史
git log --oneline
// 查看最近n个提交
git log -n
// 查看指定贡献者的提交记录
git log --author [贡献者名字]
// 图示法显示提交历史
git log --graph
// 时间正序显示提交历史
git log --reverse

// 查看配置信息
git config -l
// 设置注册github账号的邮箱
git config --global user.email "XXX@qq.com"
// 设置github账号名
git config --global user.name "tangqinwei"

// 生成新的提交
git commit -m [该提交的备注]

// 查看分支情况
git branch -avv

// 推送
git push

// 强制推送
git push -f

// 撤销最近的一次提交，将修改还原到暂存区,HEAD^^表示撤销两次提交，HEAD~n表示撤销n次提交
git reset --soft HEAD^

// 查看本地仓库所有分支的每一次版本变化
git reflog

// 回到当前分支某次提交版本
git reset --hard [版本号]
git reset --hard HEAD@{n}




```



