# Important Documentation:

#begin

Commands:
========

GO:
---

* go install
* $GOPATH/bin/hello

GIT:
---
* git init  //if you didn't clone the repo

* git clone https://github.com/favargas/hello

* git log
* git status
* git add file
* git commit -m " comments for the commit "
* git push origin master




Cofig files:
============

* ./git/config 
--------------

add bellow lines to especify the repo
    
[remote "origin"]
    url = https://github.com/favargas/hellogit
    fetch = +refs/heads/*:refs/remotes/origin/*



* .netrc 
--------

add this file to user home directory to avoid credentials


$ ls ~/.netrc 
/home/favargas/.netrc

[favargas@gbmft460 test]$ ls
mytest.go  README.md
[favargas@gbmft460 test]$ cat ~/.netrc 

machine github.com
login favargas 
password thinkPad900 



Push output:
============     
$ git push origin master
 
Counting objects: 3, done.

Delta compression using up to 4 threads.

Compressing objects: 100% (3/3), done.

Writing objects: 100% (3/3), 362 bytes | 0 bytes/s, done.

Total 3 (delta 0), reused 0 (delta 0)

To https://github.com/favargas/test

   277882a..f5d4194  master -> master
$



#end
 
