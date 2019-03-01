# Chapters 1, 2
git config
git config --global user.name "John Doe"
git config --global user.email johndoe@example.com

git help config

git clone https://github.com/libgit2/libgit2 mylibgit

git status
git status -s

git add
git add .
git add README.md

git diff
git diff --staged
git diff --cached

git commit

git rm file-3.md
git rm -f file-3.md
git rm --cached file-3.md

git mv file-4.md file-4-new.md
git mv cli-commands.md git-flow.md

git log
git log -p -2
git log --stat
git log --pretty=oneline
git log --pretty=format:"%h - %an, %ar : %s"
git log --pretty=format:"%h - %an, %ar : %s" --graph
git log --since=2.weeks
git log --since=20.minutes
git log --since=1.hours
git log -Sfunction_name

git commit --amend

# remove from stage:
git reset HEAD file-1.md

# remove changes:
git checkout -- file-1.md

git remote
git remote -v
git remote show origin
git remote rename pb paul
git remote rm paul

git fetch

git push origin master

git tag
git tag -l ‚v1.8.5*'
git tag -a v1.4 -m 'my version 1.4'
git show v1.4
git tag v1.4-lw

git config --global alias.co checkout
git config --global alias.br branch
git config --global alias.ci commit
git config --global alias.st status

# Chapter 3
git branch testing
git log --oneline --decorate
git checkout testing
git log --oneline --decorate --graph --all

git checkout -b iss53
git checkout -b hotfix

git checkout master
git merge hotfix
git branch -d hotfix
git branch -d iss53
git branch -vv
git branch --merged

git checkout -b serverfix origin/serverfix
