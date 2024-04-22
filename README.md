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

 ### Execise .2
 ```bash
 
HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (master)
$ git status 
On branch master
Your branch is up to date with 'origin/master'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        home.html

nothing added to commit but untracked files present (use "git add" to track)

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (master)
$ git add home.html

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (master)
$ git status 
On branch master
Your branch is up to date with 'origin/master'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   home.html


HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (master)
$ git stash
Saved working directory and index state WIP on master: 71ceff4 first exercise

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (master)
$ stash list
bash: stash: command not found

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (master)
$ git stash list
stash@{0}: WIP on master: 71ceff4 first exercise

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (master)
$ git list 
git: 'list' is not a git command. See 'git --help'.

The most similar commands are
        bisect
        rev-list

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (master)
$ git stash list 
stash@{0}: WIP on master: 71ceff4 first exercise

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (master)
$ git status 
On branch master
Your branch is up to date with 'origin/master'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        about.html

nothing added to commit but untracked files present (use "git add" to track)

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (master)
$ git add .

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (master)
$ git add about.html

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (master)
$ git status 
On branch master
Your branch is up to date with 'origin/master'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html


HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (master)
$ git stash
Saved working directory and index state WIP on master: 71ceff4 first exercise

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (master)
$ git stash list 
stash@{0}: WIP on master: 71ceff4 first exercise
stash@{1}: WIP on master: 71ceff4 first exercise

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (master)
$ git status
On branch master
Your branch is up to date with 'origin/master'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        team.html

nothing added to commit but untracked files present (use "git add" to track)

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (master)
$ git add team.html

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (master)
$ git status
On branch master
Your branch is up to date with 'origin/master'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html


HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (master)
$ git stash
Saved working directory and index state WIP on master: 71ceff4 first exercise

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (master)
$ git stash list
stash@{0}: WIP on master: 71ceff4 first exercise
stash@{1}: WIP on master: 71ceff4 first exercise
stash@{2}: WIP on master: 71ceff4 first exercise

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (master)
$ git stash pop stash@{1}
On branch master
Your branch is up to date with 'origin/master'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

Dropped stash@{1} (71b7a3fb57416d4fd49e4544056978ccd6cdba09)

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (master)
$ git stash list 
stash@{0}: WIP on master: 71ceff4 first exercise
stash@{1}: WIP on master: 71ceff4 first exercise

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (master)
$ git stash pop stash@{0}
On branch master
Your branch is up to date with 'origin/master'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   team.html

Dropped stash@{0} (3659eb6d3299004a3eacb4988d4712645fe4b185)

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (master)
$ git stash 
Saved working directory and index state WIP on master: 71ceff4 first exercise

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (master)
$ git stash list 
stash@{0}: WIP on master: 71ceff4 first exercise
stash@{1}: WIP on master: 71ceff4 first exercise

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (master)
$ git stash pop stash@{1}
On branch master
Your branch is up to date with 'origin/master'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   home.html

Dropped stash@{1} (6fba24d2b508f6cc8de811f6d739b7a0b020344a)

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (master)
$ git add .

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (master)
$ git commit -m "changes on home and about"
[master 0604529] changes on home and about
 1 file changed, 11 insertions(+)
 create mode 100644 home.html

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (master)
$ git push origin master
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 440 bytes | 220.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/angep72/Gym-Git-Exercise-Solutions.git
   71ceff4..0604529  master -> master

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (master)
$ git stash list
stash@{0}: WIP on master: 71ceff4 first exercise

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (master)
$ git stash list
stash@{0}: WIP on master: 71ceff4 first exercise

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (master)
$ git stash stash@{0}
fatal: subcommand wasn't specified; 'push' can't be assumed due to unexpected token 'stash@{0}'

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (master)
$ git stash pop stash@{0}
On branch master
Your branch is up to date with 'origin/master'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   team.html

Dropped stash@{0} (6c7af3d7640564b260fca2c6a83ae515aac6718e)

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (master)
$ git reset --hard
HEAD is now at 0604529 changes on home and about

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (master)
$
```
 ## Bundle 2
 ### Execise .1
 ```bash
 HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (master)
$ git checkout -b ft/bundle-2 
Switched to a new branch 'ft/bundle-2'

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (ft/bundle-2)
$ git status
On branch ft/bundle-2
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   service.html

no changes added to commit (use "git add" and/or "git commit -a")

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (ft/bundle-2)
$ git add service.html

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (ft/bundle-2)
$ git commit -m "service page"
[ft/bundle-2 c640a9b] service page
 1 file changed, 11 insertions(+)

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (ft/bundle-2)
$ git status
On branch ft/bundle-2
nothing to commit, working tree clean

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (ft/bundle-2)
$ git push origin ft/bundle-2
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 414 bytes | 103.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote:      https://github.com/angep72/Gym-Git-Exercise-Solutions/pull/new/ft/bundle-2
remote:
To https://github.com/angep72/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/bundle-2 -> ft/bundle-2

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (ft/bundle-2)
$
```
### Execise .2
``` bash
HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (ft/service-redesign)
$ git checkout main 
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (main)
$ git pull
Already up to date.

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (main)
$ git branch 
  dev
  ft/bundle-2
  ft/service-redesign
* main
  master

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (main)
$ git checkout ft/service-redesign
Switched to branch 'ft/service-redesign'

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (ft/service-redesign)
$ git add service.html

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (ft/service-redesign)
$ git commit -m "servicepage"
[ft/service-redesign 4b7508b] servicepage
 1 file changed, 1 insertion(+), 1 deletion(-)

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (ft/service-redesign)
$ git push origin ft/service-redesign
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 315 bytes | 157.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/angep72/Gym-Git-Exercise-Solutions.git
   e13ec3d..4b7508b  ft/service-redesign -> ft/service-redesign

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (ft/service-redesign)
$ git merge main 
Auto-merging service.html
CONFLICT (content): Merge conflict in service.html
Automatic merge failed; fix conflicts and then commit the result.

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (ft/service-redesign|MERGING)
$ git merge main git add service.html
error: Merging is not possible because you have unmerged files.
hint: Fix them up in the work tree, and then use 'git add/rm <file>'
hint: as appropriate to mark resolution and make a commit.
fatal: Exiting because of an unresolved conflict.

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (ft/service-redesign|MERGING)
$  git add service.html

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (ft/service-redesign|MERGING)
$ git commit -m "service conflict resiolved"
[ft/service-redesign 289c763] service conflict resiolved

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (ft/service-redesign)
$ git push 
fatal: The current branch ft/service-redesign has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/service-redesign

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (ft/service-redesign)
$ git push --set-upstream origin ft/service-redesign
Enumerating objects: 1, done.
Counting objects: 100% (1/1), done.
Writing objects: 100% (1/1), 227 bytes | 113.00 KiB/s, done.
Total 1 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/angep72/Gym-Git-Exercise-Solutions.git
   4b7508b..289c763  ft/service-redesign -> ft/service-redesign
branch 'ft/service-redesign' set up to track 'origin/ft/service-redesign'.

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (ft/service-redesign)
```

 