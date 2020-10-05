# Git Commands

![version control](https://101droid.files.wordpress.com/2015/09/versioncontrol-server.png)
![git commands](https://d1jnx9ba8s6j9r.cloudfront.net/blog/wp-content/uploads/2016/11/Git-Architechture-Git-Tutorial-Edureka-2-768x720.png)

## git init
First you must indicate that a project is going to start using git with `git init`.
```bash
cd Desktop
cd projectFolderName
git init
```
Or you can also right click on the folder >> Git Bash Here >> `git init`

## git status
To find out what status my files are in, use the `git status` command.
The states can be:
- Local
    - On working directory.
    - On staging area.
    - On local repo.
- Remote
    - On remote repo.
```bash
git status
```
## git add <file>
To add the data from the *working directory* to the *staging area*, use `git add nameFile.extent`.
```bash
git add main.cc
```
`git add .` will add all the content of the file

## git commit
To add the data from the *staging area* to the *local repo*, use `git commit -m "a brief description"`.
```bash
git commit -m "first commit"
```
It is recommended that you add a brief description of the changes you made for this commit.
It is necessary the first time to add an email and user name to know which developer makes the commits.
```bash
git config --global user.email "sample.address@gmail.com"
git config --global user.name "Name Surname1 Surname2"
```
## git diff <file>
We can use the `git diff fileName.extent` command to see the differences (changes) that have occurred in the code file.
- \+ added
- \- removed
```bash
git status
git diff main.cc
```
## git checkout - - <file>
Returns the code to an earlier version than the current one in status. We can do this using the `git checkout --fileName.extent` command.
```bash
git checkout --main.cc
```
## git log
If you want to save the code that differentiates each commit so that you can reverse the changes to that version in the future, use `git log`.
```bash
git log
```
It includes:
- A hash of the version.
- The author's name.
- The author's email.
- The date the commit was made.

## git push
To move the data from the *local repo* to the *remote repo*, use `git push`.
```bash
git push
```
## git clone <http address>
To make a copy from the central server where all the code files are to your computer to start working. Use: `git clone https://github.com/UserName/ProjectName`.
```bash
git clone https://github.com/DanielRam94m/My-CC-Notes
```
## git pull
In case several developers are working on the same remote repository, the `git pull` command brings you the changes that other developers have made.
```bash
git pull
```
When it is the first time you do a git pull you could consider doing a `git pull origin`
```bash
git pull origin
```
## git branch
```bash
git branch -a
```
## git checkout <branch>
If you want to move from one branch to another use `git checkout branchName`
```bash
git checkout dev-a
git checkout dev-b
git checkout master
```
## git fetch <repository>
Fetch all of the branches from the repository. This also downloads all of the required commits and files from the other repository
```bash
git fetch master
```
## git merge
To make a merge we move to the branch we want to save the changes and use the command `git merge branchSourceName`, where branchSouceName is the name of the branch from which we will merge in.
```bash
git checkout master
git merge dev-b
```
If at the time of "merge" there are conflicts (two different versions of the same part of the code between both branches) we do the necessary changes and then we use the `git add .` command, so the changes will be moved to the *staging area*.
```bash
git add .
```
Now we can do a `git commit "A brief description"`.
You could do a `git log --oneline` in order to check if everything looks fine and there is not more conflicts.
```bash
git log --oneline
```
And then you can do a `git push`.
#
![Git Logo](https://www.ticarte.com/sites/su/styles/max/public/users/7/teaser/git-logo.png?itok=xQhWd_9g)



**Free Software, Hell Yeah!**

[//]: # (These are reference links used in the body of this note and get stripped out when the markdown processor does its job. There is no need to format nicely because it shouldn't be seen. Thanks SO - http://stackoverflow.com/questions/4823468/store-comments-in-markdown-syntax)


   [dill]: <https://github.com/joemccann/dillinger>
   [git-repo-url]: <https://github.com/joemccann/dillinger.git>
   [john gruber]: <http://daringfireball.net>
   [df1]: <http://daringfireball.net/projects/markdown/>
   [markdown-it]: <https://github.com/markdown-it/markdown-it>
   [Ace Editor]: <http://ace.ajax.org>
   [node.js]: <http://nodejs.org>
   [Twitter Bootstrap]: <http://twitter.github.com/bootstrap/>
   [jQuery]: <http://jquery.com>
   [@tjholowaychuk]: <http://twitter.com/tjholowaychuk>
   [express]: <http://expressjs.com>
   [AngularJS]: <http://angularjs.org>
   [Gulp]: <http://gulpjs.com>

   [PlDb]: <https://github.com/joemccann/dillinger/tree/master/plugins/dropbox/README.md>
   [PlGh]: <https://github.com/joemccann/dillinger/tree/master/plugins/github/README.md>
   [PlGd]: <https://github.com/joemccann/dillinger/tree/master/plugins/googledrive/README.md>
   [PlOd]: <https://github.com/joemccann/dillinger/tree/master/plugins/onedrive/README.md>
   [PlMe]: <https://github.com/joemccann/dillinger/tree/master/plugins/medium/README.md>
   [PlGa]: <https://github.com/RahulHP/dillinger/blob/master/plugins/googleanalytics/README.md>
