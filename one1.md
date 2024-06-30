`
GIT CODE :
      git config --global user.name "shabbir811"
      git config --global user.email "email"
      git config --list
      git log                         (to check all commit history on cmd)

clone cmd: cloning a repo on our local machine.
       git clone https link


status cmd: display the state od the code.
       git status
       ls -a                (to show all file list) 

Add & commit:
        add: adds new or changed files in your working directory to the Git staging area.

        git add  filename                                      ( to add a file to staged )
        git commit -m  "some message"                          (to commit a file with msg)
        git add .                                              (to add all files at once)

Push cmd:
        push: upload local repo content to remote repo.

        git push origin main


commands for new projects and code:
          git init
          git remote add origin   (link)
          git remote  -v          (to varify remote).
          git branch              (to check branch).
          gitbranch -M main       (to rename branch)
          git push -u origin main (to push codes to same repo)
          git push origin main     

WORK FLOW:
    local git:
          1. create files/repo on github .
          2.  clone the repo
          3. we perforn some changes .
          4. then add changes 
          5.then commit changes
          6.then push to the github.


GIT BRANCHES:
    branch command:
             git branch                                (to check branch)
             git branch -M main                        (to rename branch)
             git  checkout branchName.                 (to navigate one branch to another branch)
             git checkout -b newBranchName.            (to create new branch)
             git branch -d branchName                  (to delete branch)

MERGING BRANCHES CODE:
way 1 : 
              git diff   branchName                          (to differences and compare  commits, branches, files & more ) 
              git merge  fileName                            ( to merge 2 branches ) 
way 2 : 
               create a PR
pull request (PR):
               it lets you tell others about  changes you've pushed to a branch in a repo on github.

PULL COMMAND: 
               git pull origin main 

used to fetch and download content from a remote repo  and immediately update the local repo to match that content .


RESOLVING MERGE CONFLICTS: 
an event that takes place when Git is unable to automatically  resolve difference in code b/w two commits.
 

UNDOING CHANGES: 
case1: staged changes 
                 git reset  fileName 
                 git reset

csse2: commited changes(for one commit)
                 git reset HEAD-1

case3:   commited changes(for many commits)
                  git reset  commitHash
                  git reset --hard commitHash


FORK:
a fork is a new repository that shares code and visibility settings with orignal "upstream" repository.
fork is a rough copy.

TO MOVE GITHUB FILES TO NEW REPO:
git mv   path/to/file           path/to/destination/folder






git status                              for check git status 
git init                                for  initilaze git in folder
git add  <filename>                     for track file / stage the file
git add .                               for track all files / stage all files
git commit -m "message"                 for commit
git log
git log -oneline
git branch                              for lists of branches
git branch <name>                       for create a new branch 
git switch <name>                       for swithching into branches 
git checkout <name>                     for swithching into branches 
git switch -c <name>                    for create & swithch in branch
git branch -m <old name> <new name>     for rename branch
git branch -d <name>                    for delete branch
git merge <branch name>                 for merging two branches