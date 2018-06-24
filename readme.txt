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
