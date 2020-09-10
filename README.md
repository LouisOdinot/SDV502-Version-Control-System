# SDV502-Version-Control-System
Version Control System

<b>Cherry-pick</b> 

This is a command that enables specified Git commits to be picked by the commit reference number and appended to the current master.
This is a useful way of rolling back commits if there has been an issue with a commit.

Step one - use git log to see the commit hashes

<img src="images\cp_pic1.PNG" />

Step two - use git cherry-pick d33c8d1 to move to that commit

<img src="images\cp_pic2.PNG" />

Step three - encountered merge conflicts

<img src="images\cp_pic3.PNG" />

Step four - accept the incoming change in the code

Step five - use git add and git commit to stage the changes

Step six - cherry-picked change is completed 

<img src="images\cp_pic4.PNG" />

<b>Unstaging</b> 

If you have accidentally staged all your changed files you can unstage them all by using git reset.  This should put you back in the state you were before staging all your changes files. Allowing you to stage changed files individually before you commit.

<img src="images\unstaginggitstatus.png" />

Git status.  Git status before staging and unstaging.

<img src="images\gitresetheadaddition.png" />

Git reset HEAD addition.js.  Unstages changes.

<img src="images\gitresetheadaddition.png" />

Revert the file back to the state it was in before the changes.

<b>Undoing</b> 

One of the common undos takes place when you commit too early and possibly forget to add some files, or you mess up your commit message. If you want to redo that commit, make the additional changes you forgot, stage them, and commit again using the --amend option

<img src="images\gitaddundoingthings.png" />

git add

<img src="images\gitcommitundoing.png" />

git commit -m “message”

<img src="images\gitadditionundoing.png" />

git add file

<img src="images\gitammendundoing.png" />

<b>Unmodifying</b> 

What if you realize that you don’t want to keep your changes to the CONTRIBUTING.md file? How can you easily unmodify it — revert it back to what it looked like when you last committed

<img src="images\1unmodadd addition js.png" />

git add filename

<img src="images\2 umod git checkout.png" />

git checkout – filename

<img src="images\3 git status.png" />

git status
<b>Rebase</b>

this is a command that can be used to move or combine a sequence of commits to a new base commit,  this means all the commits made in a divergent branch can be added back to the master.

Step one - Checkout to the diverged branch

<img src="images\rebase_pic1.PNG" />

Step two - Rebase to master (addeds newer commits)

<img src="images\rebase_pic2.PNG" />

Step three - Checkout to master

<img src="images\rebase_pic3.PNG" />

Step five - Merge master (no change, already up to date)

<img src="images\rebase_pic4.PNG" />

<b>Stash</b>

This is a command that can be used to store work without having to stage and commit it, 
for example if work was in progress on a branch but was not ready to be staged, then this would be a good way to preserve it without having stage it

Step one - Checkout a diverged branch and make some changes then use git status to display the state of the changes (unstaged)

<img src="images\stash_pic1.PNG" />

Step two - Use git stash to save the changes

<img src="images\stash_pic2.PNG" />

Step three - Then able to navigate to other branches without any issues

<img src="images\stash_pic3.PNG" />

Step four - Use git stash list to show the stashed work

<img src="images\stash_pic4.PNG" />

step five - Navigate back to the diverged branch and use git stash apply to unstash the saved work

<img src="images\stash_pic5.PNG" />