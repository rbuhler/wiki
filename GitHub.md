# GITHUB

##  REFERENCES
* [GUIDES](https://git-scm.com/docs)
````
Quick reference guides
````
* [reset](https://git-scm.com/docs/git-reset) : Reset local repository to remote
```
$ git reset --hard origin/master
```

* [fetch](https://git-scm.com/docs/git-fetch) :
````
$ git fetch origin master
````

## SCENARIOS
### MOVE CHANGES FROM dev TO master
```
git checkout master
git checkout dev .
git status
git add .
git commit -m "commit"
```
###  RESET master TO origin/master
```
git fetch origin
git reset --hard origin/master
```

## CONFIGURATION
- List Global Config
````
$ git config --list
````
- Set/UnSet Proxy Configuration
````
git config --global http.proxy http://proxy:8083
git config --global --unset http.proxy
````
- List Proxy Configuration
````
git config --global --get http.proxy
````

### TEMPLATE .gitconfig
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
