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

* IVORY [bitbucket.org](https://bitbucket.org/gbmnet/ivory)
* https://favargas@bitbucket.org/gbmnet/ivory.git






#### GIT and github.com:

##### MASTER:

* git init  _________//if you didn't clone the repo

* git clone https://github.com/favargas/hello

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
* git remote set-url origin https://github.com/favargas/gitdoc
* mv hellogit gitdoc
'''
[favargas@gbmft460 hellogit]$ 
'''

##### REPLACE LOCAL CHANGES:

* git checkout filename			_________//replaces the changes in your working tree with the last content in HEAD.
* git fetch origin  			_________//to drop all your local changes and commits, fetch the latest history 
* git reset --hard origin/master	_________//from the server and point your local master branch at it like this.


> keep adding...


### Cofig files:

#### ./git/config 

Add bellow lines to especify the repo
```    
[remote "origin"]
    url = https://github.com/favargas/hellogit
    fetch = +refs/heads/*:refs/remotes/origin/*
```


#### .netrc 

Add this file to user home directory to avoid credentials

```go
$ ls ~/.netrc 

/home/favargas/.netrc

[favargas@gbmft460 test]$ ls
mytest.go  README.md
[favargas@gbmft460 test]$ cat ~/.netrc 

machine github.com
login favargas 
password password1 
```


### Push output:

```ruby
$ git push origin master
Counting objects: 3, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 362 bytes | 0 bytes/s, done.
Total 3 (delta 0), reused 0 (delta 0)
To https://github.com/favargas/test
   277882a..f5d4194  master -> master
$
```


### **HELP**

1. Make my changes
    1. Fix bug
    2. Improve formatting
        - Make the headings bigger


- [x] Finish my changes
- [ ] Push my commits to GitHub
- [ ] Open a pull request


@github.XX/support.XX What do you think about these updates? Just enter the @organization/team-name and all members of that team will get subscribed to the issue.

@octocat :+1: This PR looks great - it's ready to merge! :shipit:


Let's rename \*our-new-project\* to \*our-old-project\*.


| First Header  | Second Header |
| ------------- | ------------- |
| Content Cell  | Content Cell  |
| Content Cell  | Content Cell  |


| Command | Description |
| --- | --- |
| git status | List all new or modified files |
| git diff | Show file differences that haven't been staged |



| Command | Description |
| --- | --- |
| `git status` | List all *new or modified* files |
| `git diff` | Show file differences that **haven't been** staged |


| Left-aligned | Center-aligned | Right-aligned |
| :---         |     :---:      |          ---: |
| git status   | git status     | git status    |
| git diff     | git diff       | git diff      |


| Name     | Character |
| ---      | ---       |
| Backtick | `         |
| Pipe     | \|        |


Visit https://github.com
Visit https://help.github.com/articles/getting-started-with-writing-and-formatting-on-github/




## **END** ##

 
