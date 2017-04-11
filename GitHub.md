# GITHUB

## ShortCut 
* Reset local repository branch to be just like remote repository HEAD
````
$ git fetch origin master
$ git reset --hard origin/master
````

## .gitconfig
```
[http]
	sslVerify = false
	proxy = http://proxy:8080
[user]
	email = rodrigo.buhler@sap.com
[https]
	proxy = http://proxy:8080
[core]
	autocrlf = true
    filemode = false
    autocrl = false
```
