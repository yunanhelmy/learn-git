Add, commit and push
====================

I've adding file-4 in this branch. You can take a look in history https://github.com/yunanhelmy/learn-git/commits/1-basic-example. What will you do :
* add file-5
* put some text on it
* commit
* push in this branch

Here is the step : 
* create file-5 and edit its content
* `git status` if you want to see the changes
* `git add file-5`
* `git commit -m "adding file-5"`
* `git push origin 1-basic-example`

### Exercise 1

Now you can exercise with this :
* add new folder named `animals`
* add 3 files, `dogs.txt`, `cats.txt`, `mouse.txt`
* puts pet name in files. Eg, `dogs.txt` will contains `Pleki` in line 1, `Shaggy` in line 2
* add the folder and commit
* now delete mouse.txt and also remove some dog names
* add it (with only 1 line command) and commit it
* push it to branch 1-basic-example

Undo and stash
====================
You will exercise how to undo your unstaged changes.

### Exercise 2
* add new folder named employees
* add file `softwareseni.txt` and add some employee name
* check the diff
* edit `dogs.txt`
* check the diff
* undo the changes in `dogs.txt`
* stash it and store to the new branch named `employee`
* add and commit , then push branch employee


