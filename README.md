# Memo

## Git Command Flow

create a git repository  
`git init`  
add the created files to repository  
`git add hoge.c`  
commit and write commit message  
`git commit -m "create the first program"`  
confirm a commit log  
`git log -p`  
add a new repository(user: egret678, repository name: 9cc) as a remote repository  
`git remote add origin https://github.com/egret678/9cc.git`  
push the local repository to remote repository in GitHub  
`git push -u origin master`  
rename a file  
`git mv hoge.c hoge_renamed.c`  
remove a file  
`git rm hoge.c`  
delete git added history of all files  
`git rm --cached -r .`  

## Docker Command

confirm docker version  
`docker version`
create a docker image named compilerbook  
`docker build -t compilerbook https://www.sigbus.info/compilerbook/Dockerfile`
use compilerbook image on interacitive mode  
`docker run --rm -it -v $HOME/C++/compiler/9cc:/9cc compilerbook`  
display all suspended images  
`docker container ls -a`  
