# git_ninja_tutorial

This file contains a list of commonly used git commands.

# Commands

<b>Configuring author name</b><br>
git config -global user.name emmad<br>

<b>Configuring author email</b><br>
git config -global user.email emmad@github.com<br>

<b>Creating a new file</b><br>
touch index.html
<br>

<b>Opening a file in Atom IDE</b><br>
Atom index.html	
<br>
<b>Creating a repo</b><br>
git init
<br>
<b>Adding/Staging all files</b><br>
git add .
<br>
<b>Unstaging a file</b><br>
git --rm index.html
<br>
<b>Commiting</b><br>
git commit -m "message"
<br>
<b>Viewing log of repo</b><br>
git log
git log --oneline
<br>
<b>Checkout</b><br>
git checkout 1we23asd
<br>
<b>Reverting: remove the commited code of 87aqs87a from head but keeps 87aqs87a	that commit in history</b><br>
git revert 87aqs87a
<br>
<b>Reset: remove all commits after this commit</b><br>
git reset 123jsd12 --hard
<br>
<b>Creating branch</b><br>
git branch feature-1
git branch -a //All branches
<br>
<b>Delete branch</b><br>
git branch -D feature-1
<br>
<b>Merge branch</b><br>
git merge feature-a     //first checout master branch then run this to merge
<br>
<b>Pushing branch</b><br>
git push url branchname
<br>
<b>Setting origin</b><br>
git remote add origin url
<br>
<b>Pulling branch</b><br>
git pull url branchname
<br>
