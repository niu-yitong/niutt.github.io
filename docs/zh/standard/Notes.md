### git

初始化git仓库，git会自动生成master分支，master分
支是项目的主分支

master--->dev

```
git branch 分支名（dev）  新建dev 分支
git branch   查看本地分支
git branch -r   查看远程的分支
git branch -a   查看所有的分支
git checkout 分支名(dev)   切换到dev分支
git checkout -b 分支名    创建并切换分支
git branch -d 分支名      删除分支
git push origin -d 分支   删除远程的分支
git stash  暂存修改，不产生历史记录
git stash pop 把暂存的修改恢复
git push=git fetch+git merge
git push=git fetch origin dev 从远程拉取代码 

git pull origin dev =>git fetch orign dev+git merge orign/dev

git tag v1.0     打tag
git tag -d v1.0  删除tag
```


```
合并代码：
    例：把dev分支上的合并到master分支上
    第一步：先要切换到master分支上   git checkout master
    第二步：合并分支      git merge dev
    第三步：git push origin master
```


    
