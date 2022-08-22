
### Git Status
```git status --short``` - Short status of files.

### Git Add
```git add .``` Add all files to stage.

### Git diff
```git diff``` - Show differences between the staged file and the untracked ones. <br />
```git diff --stage``` - Show differences between files that are in stage.

### Git Commit 
```git commit -m "[message]"``` - Commit your changes to the current branch. <br />
```git commit -am "[message]"``` - Add and Commit your changes to the current branch. <br />
```git commit -amend -m "[new-message]"``` - Fix message of last commit.

### Git Reset 
```git reset --soft HEAD^[number] ``` - Moves the HEAD to a specific previous commit and delete the other ones. <br />
```git reset --soft [commit-id]``` - Moves HEAD to a specific commit changes aren't deleted and stay on stage. <br />
```git reset --mixed [commit-id]``` - Moves HEAD to a specific commit changes aren't deleted and don't stay on stage. <br />
```git reset --hard [commit-id]``` - Moves to a specific commit and delete changes/files made after that commit. 

### Logs
```git log --oneline``` - Oneline logs. <br />
```git reflog``` - Reference logs of all the ocurrences. <br />
```git log -all``` - To show log of all branches.

### Git Checkout
```git checkout -- .``` - Rebuild the project to the previous commit. <br />
```git checkout -- [file-name]``` - Rebuild the file to the previous commit. <br />
```git checkout -b [branch-name]``` - Create a new branch and move us there. <br />
```git checkout [branch-name]``` - Move to a specific branch.

### Git Checkout Remote Branch
```git fetch origin [branch-name]``` - Fetchs data from remote to local workspace. <br />
```git checkout [branch-name]``` - Move to a specific branch.


### Git Branch 
```git branch``` - List all branches. <br />
```git branch [branch-name]``` - Create new branch. <br />
```git branch -d [branch-name] -f``` - Delete a branch.

### Git Merge
```git merge [branch-with-changes]``` - Merge a branch with other, you need to be in the branch without changes, master.

### Git Stash
Is a place where we can isolate our information and then recover it later. <br />
```git stash``` - Isolate our work in stash. <br />
```git stash save "[name]"``` - Isolate our work in stash with a specific description. <br />
```git stash pop``` - Recover the last stash and delete the stash. <br />
```git stash list``` - List all the stash's created. 
- ```--stat``` show more information. <br />

```git stash apply [stash-id]``` - Recover a specific stash. This create a new stash. <br />
```git stash drop [stash-id]``` - Drop a stash. <br />
```git stash show [stash-id]``` - Show the files modified. <br />
```git stash clear``` - Remove all stash's. 

### Git Rebase
What is used for?

 - To sort commits.
 - To fix commit messages.
 - To join commits.
 - To separate commits.

```git rebase [branch-name]``` - To sort commits between branchs, you need to be in your feature branch.

```git rebase -i HEAD~[Number of commits before head]``` - Iteractive mode
 - ```squash``` - use commit, but meld into previous commit.
 - ```reword``` - use commit, but edit the commit mesage.
 - ```edit``` - use commit, but stop for amending.
