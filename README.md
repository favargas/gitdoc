# Important Documentation:

> cambio feature_x branch
> cambio mybranch


* Learning [MarkDown](https://help.github.com/articles/basic-writing-and-formatting-syntax/)
* Learning [MarkDown Articles](https://help.github.com/articles)

## **begin**

### Commands:

#### GO:

* go install
* $GOPATH/bin/hello

> keep adding...


#### GIT:

* git init  //if you didn't clone the repo

* git clone https://github.com/favargas/hello

* git log
* git status
* git add file
* git commit -m " comments for the commit "
* git push origin master
* git pull origin master

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
password thinkPad900 
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




## **end**
 
