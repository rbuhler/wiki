BASICS
	INIT
	$ git init
	$ git remote add <repository> <https>
	$ git pull <repository> master

	REPEAT
	$ git add <file>
	$ git commit -m "\\ Comment"
	$ git push -u <repository>  master

	FRESH START

	echo "# nodeJS.buhler.OdataCRUD" >> README.md
	git init
	git add README.md
	git commit -m "first commit"
	git remote add origin https://github.com/rbuhler/nodeJS.buhler.OdataCRUD.git
	git push -u origin master

	* Push an existing repository from the command line
	git remote add origin https://github.com/rbuhler/<??>.git
	git push -u origin master

<li/>
<b>General</b>b>
<li/>
Initialize a directory
	$ git init
<li/>
Check the directory status
	$ git status
<li/>
New empty repository
	$ git remote add <repository> <https>
<li/>
Add a file to the stage
	$ git add <file>
Remove a file from stage
	$ git rm --cached <file>
<li/>
Commit changes
	$ git commit -m "\\ Comment"
Push staged changes
	$ git push -u <repository>  master
<li/>
Pull back a repository
	$ git pull <repository> master
Check differences
	$ git diff HEAD
Diff from staged files
	$ giyt diff --stated
<li/>
Switch between branches
	git checkout 'branch'
Clone a repository
 git clone <repository>.git
<li/>