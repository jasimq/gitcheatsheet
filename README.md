#####Get remote repo url
git remote show origin
  
#####Change git message before commit
git commit --amend -m "New commit message"

#####Create new branch from remote branch
git checkout -b localbranchname origin/branchname

#####Create new branch from current branch
git checkout -b newbranch

#####Viewing Unpushed Git Commits
git log origin/master..HEAD

#####delete unpushed git commits
git reset --hard HEAD~1

#####push local plugin branch to remote
git push origin plugin

#####show which remote branch is being tracked
git remote show origin

#####delete remote branch
git push origin --delete branchname

#####delete remote commit 1
git reset HEAD^ # remove commit locally 
git push origin +HEAD # force-push the new HEAD commit

#####delete remote commit 2
git revert <hash>
git push origin develop
