# Branching & Merging  

**Branching**  
*default branch name(when we run git init cmd) in git is "master", its's not a special branch just like any other branch, most people do not bother to change its name*

> **HEAD** : ptr to the local branch u are currently on  

	git branch nameOfNewBranch
⮩ creates a new branch , at latest snapshot/commit present at this time  

	git checkout existingBranchName  
	git switch existingBranchName  
⮩ to switch to other existing branch hcanges file in the dir to look that of the files in branch we switched to

	git  existingBranchName
⮩to switch to other existing branch  
⮩ changes file in the dir to like that of the branch we switched to 

	git switch -
⮩ to switch to the previously checked-out branch 
> switch ≣ checkout 

	git switch -c nameOfNewBranch
	git switch --create nameOfNewBranch
	git checkout -b nameOfNewBranch
⮩ to create a new branch & switch to it  
> -c ≣ --create

>⭐ it's better to have clean working tree(in current branch, i.e.,  no uncommitted changes) before we switch to another branch, though we can still switch if our working tree in current branch is not clean  *using techniques namely stashing, commit ammending* 
	
	git branch 
⮩ shows all branch in our repo  
⮩ prefix \* is to atttached HEAD branch

	git branch --all
⮩ shows all branch on localrepo(on our machine) as well as remote repo(e.g.on github)  

	git branch -v 
⮩ shows last commit on each branch 
  