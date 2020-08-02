# gitCommands
<remote> by default is origin but you can have others remotes

Basic Commands

Add all files  to the index
	git add .
	git add --all
	
add one file to the index
	git add <name_file>

commit added files on the local 	
	git commit -m "<message>"

Create a new branch on the local:
	git checkout -b <feature_branch_name>
	
publish the local branch to remote (if the branch alredy exist on  the remote)
	git push

Push a new branch to the remote repository:
	git push -u <remote> <feature_branch_name>


push Branch to Another Branch
	git push <remote> <local_branch>:<remote_name>

Get the changes from remote	
	git pull	
-------------------------------------------------------------

Delete remote branch
	 git push <remote> --delete <name_branch_remote>

Delete local branch
	 git branch -d <name_branch> 
	 git branch -D <name_branch> (Force)
	 
-------------------------------------------------------------
Remove file from index
	git rm --cached <filename>

Remove file (delete file)
	git rm -f <filename>

-------------------------------------------------------------

see the log/histories 
	git log --graph --oneline --decorate --all
 
	git log --graph --pretty=oneline --abbrev-commit
	
	git log (to exit press q)	
	
-------------------------------------------------------------	 
Reset stages
	
	git reset --hard HEAD <branch> 
	
	git reset --hard HEAD
	
	git reset --hard <comite number> (repository to workarea)

	git reset --hard (repository to workarea)
	
	
	undo the lest commit to working area
	git reset --mixed HEAD
	
	undo the itens on index area to working area (directory)
	git reset --mixed (repository to index) 
	
	undo the lest commit to index area
	git reset --soft HEAD^ 
	
-------------------------------------------------------------

		

		
merge
	--git merge <name_branch> <other name_branch> 
	
	git merge <other name_branch> 
	
rebase 
	on currente branch
	 
		git rebase <other branch> (the chenges will apply to current branche)

	in case of conflict -correct conflicts -
		git add . (to add the changes on index)
		git rebase --continue  (to continue the process of rebase )

delete files after change git ignore	
	git rm -r --cached .
	git add --all
	git commit -m "<ss>"

git clean -fxd

remove branchs deleted from remote
git fetch --prune

git branch | grep -v '^*' | xargs git branch -D


ADS
ads
ASD

sd
DS
das



	git diff (workarea index)
	git diff --cached (index  repository)