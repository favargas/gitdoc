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

* git checkout master #
* git pull # update local master from remote master
* git checkout <your_branch>
* git merge master # solve merge conflicts if you have`

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

 
* git config --global credential.helper store  _________//The storage represents a single %USERPROFILE%\.git-credentials

> keep adding...


##### Import an external Git repo:

1. Create a new repo:
   
2. Cone external
   ```
   $ git clone --bare https://external-host.com/EXTUSER/REPO.git
   # Makes a bare clone of the external repository in a local directory
   ```
3. Push to new repo:
   ```
   $ cd REPO.git
   $ git push --mirror https://github.com/USER/REPO.git
   # Pushes the mirror to the new repository on GitHub.com
   ```
4. Delete external repo
   ```
   cd ..
   rm -rf REPO.git
   ```


##### rename file:
```
git mv app.py myApp.py
git status

cp app.txt app1.txt
git rm app.txt
git add app1.txt
git status
git add *
git commit -m ""
```

##### TOKEN AND CREDENTIALS:
```
https://www.squash.io/how-to-authenticate-git-push-with-github-using-a-token/
https://stackoverflow.com/questions/6565357/git-push-requires-username-and-password


git config credential.helper store
git push https://github.com/owner/repo.git

Username for 'https://github.com': <USERNAME>
Password for 'https://USERNAME@github.com': <PASSWORD>

git config --global credential.helper store
git config --global credential.helper 'cache --timeout 7200'

---

<REMOTE_URL> = https://<TOKEN>@github.com/<username>/<repository>.git
git remote set-url origin <REMOTE_URL>
```

##### REMOVE COMMITS:
```
To removed the last commit using:

git reset --soft HEAD~1
I then excluded the file from the commit.

Note: Use HEAD~N to go back to N number of previous commits. (i.e. 3, 4) Always use the --soft switch to maintain changes in the folder

To commit only one file

git commit -m "gitignore add " /mypc/gbm/CajaAnde/cda-git/cda-ocp/.gitignore


You can of course also remove multiple files at once from the Staging Area:

git restore --staged *.css

```


## **END** ##


 
