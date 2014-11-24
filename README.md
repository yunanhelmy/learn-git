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
Pull the other changes using `git pull origin master`. Same goes for `git pull origin 2-working-with-git`