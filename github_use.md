#### Quick setup — if you’ve done this kind of thing before
    We recommend every repository include a README, LICENSE, and .gitignore.


#### …or create a new repository on the command line
```echo "# armeng_markdown" >> README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin git@github.com:liweigong/armeng_markdown.git
git push -u origin master
```

#### …or push an existing repository from the command line
    git remote add origin git@github.com:liweigong/armeng_markdown.git

    git push -u origin master



#### …or import code from another repository
    You can initialize this repository with code from a Subversion, Mercurial, or TFS project.


---
#### 然后本着mater空白的原则,需要创建一个dev分支，但是服务器上面没有dev分支，怎么办

##### 先本地创建dev分支
    git checkout -b dev

##### 尝试push到github上
    git push

得到错误信息如下：

    fatal: The current branch dev has no upstream branch.
    To push the current branch and set the remote as upstream, use

        git push --set-upstream origin dev

##### 根据提示,执行如下指令
    git push --set-upstream orign dev

返回结果如下

    Total 0 (delta 0), reused 0 (delta 0)
    To github.com:liweigong/armeng_markdown.git
     * [new branch]      dev -> dev
    Branch 'dev' set up to track remote branch 'dev' from 'origin'.

