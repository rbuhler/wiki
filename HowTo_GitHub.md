## Daily Work

* MOVE CHANGES FROM dev TO master
```
git checkout master
git checkout dev .
git status
git add .
git commit -m "commit"	
```
* RESET MASTER TO ORIGIN/MASTER
```
git fetch origin
git reset --hard origin/master
```

## Configuration
- List Global Config
````
$ git config --list 
````
- Set Proxy Configuration
````
git config --global http.proxy http://proxy:8083
````
- Reset Proxy Configuration
````
git config --global --unset http.proxy
````
- List Proxy Configuration
````
git config --global --get http.proxy
````

## Basic
<hr align="left"/>
	<b>INIT</b>
		$ git init
		$ git remote add &#60; repository &#62; &#60;https&#62;
		$ git pull &#60;repository&#62; master
	<b>REPEAT</b>
		$ git add <file>
		$ git commit -m "\\ Comment"
		$ git push -u &#60; repository &#62;  master

<hr align="left"/>
	<b>FRESH START</b>
	$ echo "# nodeJS.buhler.OdataCRUD" >> README.md
	$ git init
	$ git add README.md
	$ git commit -m "first commit"
	$ git remote add origin https://github.com/rbuhler/nodeJS.buhler.OdataCRUD.git
	$ git push -u origin master

<li> Push an existing repository from the command line <br>
	$ git remote add origin https://github.com/rbuhler/<??>.git
	$ git push -u origin master

<li/>
<b>General</b>
<hr align="left"/>
Initialize a directory
	$ git init
<hr align="left"/>
Check the directory status
	$ git status
<hr align="left"/>
New empty repository
	$ git remote add <repository> <https>
<hr align="left"/>
Add a file to the stage
	$ git add <file>
Remove a file from stage
	$ git rm --cached <file>
<hr align="left"/>
Commit changes
	$ git commit -m "\\ Comment"
Push staged changes
	$ git push -u <repository>  master
<hr align="left"/>
Pull back a repository
	$ git pull <repository> master
Check differences
	$ git diff HEAD
Diff from staged files
	$ giyt diff --stated
<hr align="left"/>
Switch between branches
	git checkout 'branch'
Clone a repository
 git clone <repository>.git
<hr align="left"/>
