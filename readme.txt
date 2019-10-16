创建版本库：
$ mkdir learngit //创建文件夹learngit 
$ cd learngit
$ pwd  //显示当前目录
$git init //把这个目录变成Git可以管理的仓库

换库：
$ cd 库名
（默认为SPB_Data）

$$$$$$$$$$$$$$$$$$$$$$$$$$$

加文件：
$git add <file>

提交文件：
$git commit -m "note"

查看修改内容:
$git diff <file>

$$$$$$$$$$$$$$$$$$$$$$$$$$

从近到远的提交日志:
$git log/reflog
简化：
$git log --pretty=oneline

版本时光穿梭:  
（HEAD^ or HEAD^^ or HEAD~100 or commit id）
$git reset --hard HEAD^

丢弃工作区的修改：
$git restore <file>
$git checkout -- <file>
git checkout其实是用版本库里的版本替换工作区的版本，无论工作区是修改还是删除，都可以“一键还原”。

把暂存区的修改撤销（unstage）:
$git reset HEAD <file>

git rm 来删除文件，同时还会将这个删除操作记录下来
git commit -m "abc" 提交

rm 来删除文件，仅仅是删除了物理文件
git commit -am "abc"提交

强制删除,cb文件夹是一个目录:
$rm -rf <cb>