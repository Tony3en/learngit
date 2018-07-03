Git is a distributed version control system.
Git is free software distributed under the GPL.
Git has a mutable index called stage.
Git tracks changes of files.
Creating a new branch is quick and simple.
a little modify.

//init 
1.创建新文件夹
mkdir filename
cd filename
pwd //查看文件路径
2.初始化git仓库
git init
3.创建文件&working directory
//new example.txt 
4.stage file
git add example.txt
5.
git commit -m "(message)description"
6.修改 提交 查看
git status          //查看工作区状态 
git diff            //查看修改内容

//提交 
git add filename
git commit -m "message"

//回退
before git add =>   git checkout -- filename   //discard changes in working directory
after git add =>    git reset HEAD filename  // to unstage


7.版本回退
git reset --hard HEAD^(HEAD^之前版本 HEAD^^之前两个版本  HEAD~100)
git reset --hard commit_id

git log //查看历史 确定回到历史的版本号(commit_id)
git log --pretty=oneline //一行展示
git reflog //查看历史命令 确定回到未来的那个版本的版本号(commit_id)

8.管理修改
关于stage-(缓存区)
git add ->进入stage(缓存区状态) -->git commit -->HEAD 提交到分支 --> working tree clean

9.撤销修改 checkout reset(reset-->7.版本回退)
    1.未进入缓存区(unstage->git checkout -- file  )放弃所有修改.(命令中 -- 很重要)
    2.已经添加进缓存区 即(after git add -> git reset HEAD file ->back to 1. git checkout -- file )
    3.已经修改到版本库 即(after git commit -> bakc to 7.版本回退  git reset --hard HEAD^)





