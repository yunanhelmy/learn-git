Before you read the documentation below please have a time to learn Git in :

* https://try.github.io/levels/1/challenges/1
* http://git-scm.com/doc
* http://pcottle.github.io/learnGitBranching/
* https://www.atlassian.com/git/

Basic Configuration
===================

### initialize empty git repository

`git init`


### basic configuration

`git config --global user.name "yunanhelmy"`

`git config --global user.email "yunan@softwareseni.com"`


### add new remote

`git remote add origin git@github.com:yunanhelmy/learn-git.git`


### remove remote url

`git remote remove origin`


### see the changes

`git status`



Working with Git
===================

### add file

There area several ways to add file. Usually i did :
* adding all files using `git add .`
* adding all files that have suffix using `git add ".*.html"`
* adding all files include removing deleted files using : git add -A
* add single file using `git add index.html`

### commit
Commit to staging area using `git commit -m "this is my comment"`

### push
Push to the repository using `git push origin master`. Because its just a branch you can have a command like this : `git push origin 2-working-with-git`.

### pull
Pull the other changes using `git pull origin master`. Same goes for `git pull origin 2-working-with-git`.

### diff changes
You can check the changed code using `git diff HEAD`. If you're checking new file, you can use `git diff --staged`.

### undo
Undoing before commit is easy. You can use `git checkout index.html` to undo. Or you can use git stash.

### stash
`git stash` can erase all your changes. In fact it will move your unstaged file into stash hash. 
There are several command that commonly used :
* `git stash` to stash your changes
* `git stash list` to inspect list of hash
* `git stash branch yourbranch` to move your changes into new branch. This is useful if you want to test it in another branch
* `git stash apply` to reundo your stash. This will use first stash hash 
* `git stash apply stash@{2}` to reundo your stash in index = 2

### reset
Reset will remove commit history. It is intented to  rollback into previous commit. You can use `git reset HEAD~1` to rollback 1 step. Also it's accept commit hash `git reset 123123`. Use this in local (preferred local only) or if you want your commit completely removed.

### revert
Revert is rollback to previous version too. But it will keep history and adding 1 revert commit. You can use `git revert HEAD~1` to rollback 1 step, but you'll see commit history so other developer can easily track graph. Also it's accept commit hash `git revert 123123`. Use this revert if you're collaborating with team, all progress can be viewed in history.

### branch
There are several commands for branching :
* create new branch using `git branch myhotfix`
* then `git checkout myhotfix` to move into your branch
* `git checkout -b myhotfix` to create new branch and move to that branch
* `git merge myhotfix` to merge myhotfix branch with your current branch

### rebase
Rebase used to track commits and implement it to another branch. Rebase is like copy all commit into another branch. You can rebase myhotfix with master `git rebase master`. It will implement master commit into myhotfix

### cherry-pick
You can implement specific commit from other branch using `git cherry-pick 123123`

### log
There area several commands in log :
* `git log` will show basic log history
* `git log --oneline` is the simple one line log
* `git log --oneline --decorate` if you want more beatiful log
* `git log --graph --oneline --decorate` will print graph
* `git shortlog` is simple short log

### tips