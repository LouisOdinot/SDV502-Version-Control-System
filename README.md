# SDV502-Version-Control-System
Version Control System

<b>git cherry-pick</b> 

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


