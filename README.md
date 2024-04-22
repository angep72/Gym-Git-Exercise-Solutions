# Git Exercises
## Bundle 1
### Execise .1
```bash 
$ git init
Reinitialized existing Git repository in C:/Users/HP/git-exercises/.git/

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (master)
$ git branch -M main

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (main)
$ git branch -M master

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (master)
$ git status 
On branch master
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (master)
$ git add README.md

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (master)
$ git status 
On branch master
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   README.md


HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (master)
$ git commit -"mastering git codes"
[master 9479c59] astering git codes
 1 file changed, 1 insertion(+), 1 deletion(-)

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (master)
$ git status
On branch master
nothing to commit, working tree clean

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (master)
$ git remote add origin https://github.com/angep72/Gym-Git-Exercise-Solutions.git
error: remote origin already exists.

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (master)
$ git push
fatal: The current branch master has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin master

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (master)
$     git push --set-upstream origin master
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (6/6), 507 bytes | 169.00 KiB/s, done.
Total 6 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/angep72/Gym-Git-Exercise-Solutions.git
 * [new branch]      master -> master
branch 'master' set up to track 'origin/master'.

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (master)
$ git checkout -b dev
Switched to a new branch 'dev'

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (dev)
$ git push 
fatal: The current branch dev has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin dev

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (dev)
$ git push --set-upstream origin dev
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote: 
remote: Create a pull request for 'dev' on GitHub by visiting:
remote:      https://github.com/angep72/Gym-Git-Exercise-Solutions/pull/new/dev
remote:
To https://github.com/angep72/Gym-Git-Exercise-Solutions.git
 * [new branch]      dev -> dev
branch 'dev' set up to track 'origin/dev'.

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (dev)
$ git checkout -b test
Switched to a new branch 'test'

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (test)
$ git checkout dev
Switched to branch 'dev'
Your branch is up to date with 'origin/dev'.

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (dev)
$ git branch -d test
Deleted branch test (was 9479c59).

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (dev)
$ git push 
Everything up-to-date

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (dev)
$
 ```