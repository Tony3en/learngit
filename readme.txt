Git is a distributed version control system.
Git is free software distributed under the GPL.
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