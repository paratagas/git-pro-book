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

git reset HEAD file-1.md
