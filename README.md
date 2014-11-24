Brancing, merging, rebasing, cherry-picking, gitignore
======================================================

Oops i think we have unused branch named 3-branch-test. Can you delete it?

I've create branch `3-branch`. Hopefully you remember how to create a branch. I create this branch with `git checkout -b 3-branch origin/master`. 

### Exercise 5 
* now please create 2 branch named `3-branch-reset` and `3-branch-revert`
* checkout `3-branch-reset` and reset this branch to 700a18451d3d6229197e6c9fb527b3f2a9596b01
* push `3-branch-reset`
* checkout `3-branch-revert` and revert this branch to `3-branch-revert`
* push `3-branch-revert`

You can see the difference between reset and revert.

### Exercise 6
We will learn how to rebase `3-branch` onto master. `3-branch` is ahead of 1 commit from master and we want it synced.
* checkout `3-branch`
* rebase `3-branch` with `git rebase master`
* see the graph
* push

### Exercise 7
We will learn how to pick specific commit using cherry-pick
* checkout branch `2-collaborate`
* pick this commit 1ed219bc3298f768df02d709919ef4df199a7b9d (from master)
* push

### Excercise 8
Ok now we have to ignoring the changes in file-2. But file-2 already exist. Lets do gitignore
* create new branch
* add file .gitignore
* add line that exclude the file-2
* remove index repository file-2
* commit gitignore
* merge to all branch


