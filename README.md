# GO and GIT Documentation:


* Learning [MarkDown](https://help.github.com/articles/basic-writing-and-formatting-syntax/)
* Learning [MarkDown Articles](https://help.github.com/articles)

## **BEGIN**

### Commands:

#### GO:
* Go Lang [golang.org](https://golang.org/)
* Learn Go Code [Go Code](https://golang.org/doc/code.html)

* go install
* $GOPATH/bin/hello

> keep adding...

#### Bitbucket.org 


#### GIT and github.com:

##### MASTER:

* git init  _________//if you didn't clone the repo

* git clone https://github.com/user/hello

* git log
* git status
* git add file
* git commit -m " comments for the commit "
* git push origin master
* git pull origin master

* git pull origin master __________//to merge origin and remote

* git remote add origin >"remote repository URL"
* git remote -v
* git pussh origin master

* git rm --cached installers/jdk-8u131-linux-x64.rpm
* git rm installers/jdk-8u131-linux-x64.rpm

* git commit --amend -CHEAD

* git checkout
* git reset HEAD installers/jdk-8u131-linux-x64.rpm __________//rollback

* git show
* git rm -r --cached .
* git add .
* git commit -m "fixed untracked files"


* Push ignored and deleted files [push-ignored-deleted](https://stackoverflow.com/questions/33466466/git-still-trying-to-push-ignored-and-deleted-file)
* Purging a file from repository's history [filter-bransh](https://help.github.com/articles/removing-sensitive-data-from-a-repository/)

```
git filter-branch --force --index-filter \
'git rm --cached --ignore-unmatch installers/jdk-8u131-linux-x64.rpm' \
--prune-empty --tag-name-filter cat -- --all
```



##### BRANCHES:

* git checkout -b mybranch  _________//new branch.
* git checkout master       _________//switch to master.
* git push origin mybranch  _________//push branch to repo, to make it avilable to others.
* git branch -d mybranch    _________//delete branch from local.
* git push origin :mybranch	_________//delete branch from remote.

* git show		_________//show changes. 
* git branch		_________//show branches.
* git branch -a
* git branch -r

* git fetch -p = git pull -p  _________//then remote branches will be pruned.



##### UPDATE & MERGE:

* git pull		_________//update local repo to the newest commit, to fetch and merge remote changes.
* git merge <branch>	_________//to merge another branch into your active branch (e.g. master).

* git add <filename>	_________//in case of any conflict.

* git diff <source_branch> <target_branch> 	_________//preview changes before merging.

##### TAGGING:

* git tag 1.0.0 1b2e1d63ff	_________//for software releases. create a new tag named 1.0.0, the 1b2e1d63ff stands for the first 10 characters of the commit id.


##### LOG:

* git log
* git log --author=bob
* git remote set-url origin https://github.com/user/gitdoc
* mv hellogit gitdoc
'''

'''

##### REPLACE LOCAL CHANGES:

* git checkout filename			_________//replaces the changes in your working tree with the last content in HEAD.
* git fetch origin  			_________//to drop all your local changes and commits, fetch the latest history 
* git reset --hard origin/master	_________//from the server and point your local master branch at it like this.


> keep adding...



## **END** ##


 
