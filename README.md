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

