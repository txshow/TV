# 更新命令

1、在github上创建项

2、使用git clone git@github.com:txshow/CatVodTV.git 克隆到本地

3、编辑项目

4、git add . （将改动添加到暂存区）

5、git commit -m "update jar"

6、git push origin master 将本地更改推送到远程master分支。

#恢复历史

1、用命令行模式 先查看版本号：git reflog或者git log --pretty=oneline

2、用命令行模式 恢复到某个版本号：git reset --hard <commit ID号>

3、推送到远程：githubgit push -f -u origin master

#ssh key获取

1、配置账户

git config --global user.name “your_username”  #设置用户名

git config --global user.email “your_registered_github_Email”  #设置邮箱地址

2、生成key

ssh-keygen -t rsa -C "your email"

3、复制key

cd ~/.ssh

cat ~/.ssh/id_rsa.pub
