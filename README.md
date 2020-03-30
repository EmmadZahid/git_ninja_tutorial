# git_ninja_tutorial

This file contains a list of commonly used git commands. In order to use command prompt for git, run Git Bash.
For further please see the video tutorials of this playlist https://www.youtube.com/playlist?list=PL4cUxeGkcC9goXbgTDQ0n_4TBzOO0ocPR
For common mistakes: https://www.youtube.com/watch?v=FdZecVxzJbk
For git stash: https://www.youtube.com/watch?v=KLEDKgMmbBI
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
<b>Delete branch (it will delete locally)</b><br>
git branch -d feature-1
<br>
<b>Delete branch from origin</b><br>
git push origin --delete feature-1
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
<b>Checking origin url</b><br>
git remote -v
git remote show origin
<br>
<b>Checking Difference</b><br>
git diff   //To check changes before commiting<br>
git diff 12wsqw 34rf34r
<br>
<b>Removing the local changes- It will remove all the local changes in test4.txt</b><br>
git checkout test4.text
<br>
<b>If you forgot to add files in previous commit</b><br>
git commit --amend<br>
after that type wq. Note that commit has will change in this case
<br>
<b>Stat of log</b><br>
git log --stat
<br>
<b>If commit was accidently done in wrong branch</b><br>
git checkout correctbranch<br>
git cherry-pick 123qws12  //this is hash of the commit that was done in wrong branch
<br>

<b>Ref log: it shows all the commands that you have run</b><br>
git reflog
<br>

<b>Want to revert any commit</b><br>
git revert 1q2w123  //It will add one more commit on top that will completely undo all of that changes of 1q2w123
<br>
<b>Reset</b><br>
git reset --soft 1231sqw    //It will remove the commit but will move those files to stage
git reset 1231sqw           //It will remove the commit but files will be untracked
git reset --hard 1231sqw    //It will remove the commit and all files
<br>
git log --all --oneline --graph
<br>
<b>To see the file changes at specific commit</b>
<br>
git show commit -- path
<br>
<b>To see the fetched commits</b>
<br>git log --all<br>
<b>To see the files changes in commit</b>
<br>git show 43r34j3f384jr83j4r<br>
<b>To see only the files in log</b>
<br>git log --stat --all<br>
<b>Tagging a commit </b>
<br>
git tag -a v1.4 -m "message"<br>
git push origin tagname<br>
<b>Deleting a tag</b>
<br>
  <b>Discarding unstagged files</b><br>
  git checkout -- .
  <br>
  <b>Discarding untracked files</b><br>
  git clean -df
    <br>
  <b>Cherry pick specific file</b><br>
  git cherry-pick -n <commit>         It will not commit. Once done, remove the files which are not required
  <br>
  
  <br>
  <b>Stash save</b><br>
  git stash save "message"
  <br>
  
  <br>
  <b>Stash list</b><br>
  git stash list

  <br>
  <b>Stash apply</b><br>
  git stash apply stash@{0} //it does not delete the stash
  <br>
  <b>Stash apply</b><br>
  git stash pop //it delets the stash and put top most on code
  <br>
  <b>Stash drop(CAREFULLY)</b><br>
  git stash drop stash@{0} //If you apply stash{0} and then want to revert you will do this command
  <br> 
  <br>
  <b>Stash show</b><br>
  git stash show
  <br> 
  <br>
  <b>Stash show content</b><br>
  git stash show -p
  <br> 
  <b>Stash show content of specific stash</b><br>
  git stash show -p stash@{1}
  <br> 
  
  
