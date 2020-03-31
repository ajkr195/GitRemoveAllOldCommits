# GitRemoveAllOldCommits
<h4>  GitRemove All Old Commits. Keep only last commit. </h4> 


<h4> Create a temporary branch and checkout:</h4>
$ git checkout --orphan temp_branch

<h4> Add all files to the temporary branch and commit the changes:</h4>
$ git add -A

$ git commit -am "initial"

<h4> Delete the master branch:</h4>
$ git branch -D master


<h4> Rename the temporary branch to master:</h4>
$ git branch -m master

<h4> Forcefully update the remote repository: </h4> 
$ git push -f origin master
