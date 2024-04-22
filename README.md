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
##Bundle 3
### Execise .1
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
 
 ###Exercise 1:
 ```bash 
 
HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (main)
$ git checkout -b ft/team-page
Switched to a new branch 'ft/team-page'

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (ft/team-page)
$ git add team.html

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (ft/team-page)
$ git push 
fatal: The current branch ft/team-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/team-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (ft/team-page)
$ git push --set-upstream origin ft/team-page
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote: 
remote: Create a pull request for 'ft/team-page' on GitHub by visiting:
remote:      https://github.com/angep72/Gym-Git-Exercise-Solutions/pull/new/ft/team-page
remote:
To https://github.com/angep72/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/team-page -> ft/team-page
branch 'ft/team-page' set up to track 'origin/ft/team-page'.

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (ft/team-page)
$ git checkout main
Switched to branch 'main'
M       team.html
Your branch is up to date with 'origin/main'.

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (main)
$ git checkut -b ft/contact-page
git: 'checkut' is not a git command. See 'git --help'.

The most similar command is
        checkout

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (main)
$ checkout -b ft/contact-page
bash: checkout: command not found

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (main)
$ git checkout -b ft/contact-page
Switched to a new branch 'ft/contact-page'

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (ft/contact-page)
$ git checkout ft/team-page
Switched to branch 'ft/team-page'
M       team.html
Your branch is up to date with 'origin/ft/team-page'.

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (ft/team-page)
$ git log
commit 01ae7a25b2a343b862acfb07c942f9173edaf56a (HEAD -> ft/team-page, origin/main, origin/ft/team-page, main, ft/contact-page)
commit 01ae7a25b2a343b862acfb07c942f9173edaf56a (HEAD -> ft/team-page, origin/main, origin/ft/team-page, main, ft/contact-page)
Author: angep72 <p.umunyana@alustudent.com>
commit 01ae7a25b2a343b862acfb07c942f9173edaf56a (HEAD -> ft/team-page, origin/main, origin/ft/team-page, main, ft/contact-page)
Author: angep72 <p.umunyana@alustudent.com>
Date:   Mon Apr 22 16:10:15 2024 +0200

    done with exercice bundle 2

commit e0f3d6d3817f1d28c757c0581f2c02843c1c0c88
Author: angep72 <p.umunyana@alustudent.com>
Date:   Mon Apr 22 15:41:33 2024 +0200

    services

commit 18393c7d9c33b6c3ee58a0ec746037627d8bac54

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (ft/team-page)
$ git checkout -b ft/contact-page
fatal: a branch named 'ft/contact-page' already exists

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (ft/team-page)
$ git checkout ft/contact-page
Switched to branch 'ft/contact-page'
M       team.html

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (ft/contact-page)
$ git add .

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (ft/contact-page)
$ git commit -m "contact page"
[ft/contact-page a2913fe] contact page
 2 files changed, 13 insertions(+), 3 deletions(-)
 create mode 100644 contact.html

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (ft/contact-page)
$ git push 
fatal: The current branch ft/contact-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/contact-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (ft/contact-page)
$ git push --set-upstream origin ft/contact-page
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 8 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 497 bytes | 497.00 KiB/s, done.
Total 4 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/contact-page' on GitHub by visiting:
remote:      https://github.com/angep72/Gym-Git-Exercise-Solutions/pull/new/ft/contact-page
remote:
To https://github.com/angep72/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/contact-page -> ft/contact-page
branch 'ft/contact-page' set up to track 'origin/ft/contact-page'.

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (ft/contact-page)
$ git log
commit a2913fe7cc53cf6baa1fa16d3cfe21d4ab0934bf (HEAD -> ft/contact-page, origin/ft/contact-page)
Author: angep72 <p.umunyana@alustudent.com>
Date:   Mon Apr 22 16:48:46 2024 +0200

    contact page

commit 01ae7a25b2a343b862acfb07c942f9173edaf56a (origin/main, origin/ft/team-page, main, ft/team-page)
Author: angep72 <p.umunyana@alustudent.com>
Date:   Mon Apr 22 16:10:15 2024 +0200

    done with exercice bundle 2

commit e0f3d6d3817f1d28c757c0581f2c02843c1c0c88

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (ft/contact-page)
$ git cherry-pick a2913fe7cc53cf6baa1fa16d3cfe21d4ab0934bf
The previous cherry-pick is now empty, possibly due to conflict resolution.
If you wish to commit it anyway, use:

    git commit --allow-empty

Otherwise, please use 'git cherry-pick --skip'
On branch ft/contact-page
Your branch is up to date with 'origin/ft/contact-page'.

You are currently cherry-picking commit a2913fe.
  (all conflicts fixed: run "git cherry-pick --continue")
  (use "git cherry-pick --skip" to skip this patch)
  (use "git cherry-pick --abort" to cancel the cherry-pick operation)

nothing to commit, working tree clean

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (ft/contact-page|CHERRY-PICKING)
$ git add .

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (ft/contact-page|CHERRY-PICKING)
$ git commit -m "new changes in contact page "
[ft/contact-page 0be6377] new changes in contact page
 Date: Mon Apr 22 16:48:46 2024 +0200
 1 file changed, 1 insertion(+), 1 deletion(-)

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (ft/contact-page)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 339 bytes | 339.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/angep72/Gym-Git-Exercise-Solutions.git
   a2913fe..0be6377  ft/contact-page -> ft/contact-page

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (ft/contact-page)
$ git checkout -b ft/faq-page
Switched to a new branch 'ft/faq-page'

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (ft/faq-page)
$ git add .

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (ft/faq-page)
$ git commit -m "faq page"
[ft/faq-page 39d9a02] faq page
 1 file changed, 11 insertions(+)
 create mode 100644 faq.html

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (ft/faq-page)
$ git push 
fatal: The current branch ft/faq-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/faq-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (ft/faq-page)
$ git push --set-upstream origin ft/faq-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 424 bytes | 424.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/faq-page' on GitHub by visiting:
remote:      https://github.com/angep72/Gym-Git-Exercise-Solutions/pull/new/ft/faq-page
remote:
To https://github.com/angep72/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/faq-page -> ft/faq-page
branch 'ft/faq-page' set up to track 'origin/ft/faq-page'.

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (ft/faq-page)
$ git log
commit 39d9a02de780fb95f5fa6e716e8d56e0b78d7cff (HEAD -> ft/faq-page, origin/ft/faq-page)
Author: angep72 <p.umunyana@alustudent.com>
Date:   Mon Apr 22 16:57:40 2024 +0200

    faq page

commit 0be63775d330ae8df873779c0a6aad94d224a4a8 (origin/ft/contact-page, ft/contact-page)
Author: angep72 <p.umunyana@alustudent.com>
Date:   Mon Apr 22 16:48:46 2024 +0200

    new changes in contact page

commit a2913fe7cc53cf6baa1fa16d3cfe21d4ab0934bf

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (ft/faq-page)
$ git revert a2913fe7cc53cf6baa1fa16d3cfe21d4ab0934bf
CONFLICT (modify/delete): contact.html deleted in parent of a2913fe (contact page) and modified in HEAD.  Version HEAD of contact.html left in tree.
error: could not revert a2913fe... contact page
hint: After resolving the conflicts, mark them with
hint: "git add/rm <pathspec>", then run
hint: "git revert --continue".
hint: You can instead skip this commit with "git revert --skip".
hint: To abort and get back to the state before "git revert",
hint: run "git revert --abort".

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (ft/faq-page|REVERTING)
$ git log
commit 39d9a02de780fb95f5fa6e716e8d56e0b78d7cff (HEAD -> ft/faq-page, origin/ft/faq-page)
Author: angep72 <p.umunyana@alustudent.com>
Date:   Mon Apr 22 16:57:40 2024 +0200

    faq page

commit 0be63775d330ae8df873779c0a6aad94d224a4a8 (origin/ft/contact-page, ft/contact-page)
Author: angep72 <p.umunyana@alustudent.com>
Date:   Mon Apr 22 16:48:46 2024 +0200

    new changes in contact page

commit a2913fe7cc53cf6baa1fa16d3cfe21d4ab0934bf

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (ft/faq-page|REVERTING)
$ git revert 0be63775d330ae8df873779c0a6aad94d224a4a8
error: Reverting is not possible because you have unmerged files.
hint: Fix them up in the work tree, and then use 'git add/rm <file>'
hint: as appropriate to mark resolution and make a commit.
fatal: revert failed

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (ft/faq-page|REVERTING)
$ git status
On branch ft/faq-page
Your branch is up to date with 'origin/ft/faq-page'.

You are currently reverting commit a2913fe.
  (fix conflicts and run "git revert --continue")
  (use "git revert --skip" to skip this patch)
  (use "git revert --abort" to cancel the revert operation)

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   team.html

Unmerged paths:
  (use "git restore --staged <file>..." to unstage)
  (use "git add/rm <file>..." as appropriate to mark resolution)
        deleted by them: contact.html


HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (ft/faq-page|REVERTING)
$ git add contact.html

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (ft/faq-page|REVERTING)
$ git commit -m "resolved umerged"
[ft/faq-page df126d5] resolved umerged
 1 file changed, 3 insertions(+), 2 deletions(-)
This reverts commit 0be63775d330ae8df873779c0a6aad94d224a4a8.

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (ft/faq-page)
$ git revert 0be63775d330ae8df873779c0a6aad94d224a4a8
^C

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (ft/faq-page)
$ ^C

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (ft/faq-page)
$ ^C

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (ft/faq-page)
$ git revert 0be63775d330ae8df873779c0a6aad94d224a4a8
[ft/faq-page 61398a1] Revert "new changes in contact page"
 1 file changed, 1 insertion(+), 1 deletion(-)

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (ft/faq-page)
$ git push
Enumerating objects: 9, done.
Counting objects: 100% (9/9), done.
Delta compression using up to 8 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 670 bytes | 670.00 KiB/s, done.
Total 6 (delta 4), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (4/4), completed with 3 local objects.
To https://github.com/angep72/Gym-Git-Exercise-Solutions.git
   39d9a02..61398a1  ft/faq-page -> ft/faq-page

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (ft/faq-page)
$
```

### Exercise 2
``` bash
HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (ft/faq-page)
$ git branch checkout -b ft/home-page-redesign
error: unknown switch `b'
usage: git branch [<options>] [-r | -a] [--merged] [--no-merged]
   or: git branch [<options>] [-f] [--recurse-submodules] <branch-name> [<start-point>]
   or: git branch [<options>] [-l] [<pattern>...]
   or: git branch [<options>] [-r] (-d | -D) <branch-name>...
   or: git branch [<options>] (-m | -M) [<old-branch>] <new-branch>
   or: git branch [<options>] (-c | -C) [<old-branch>] <new-branch>
   or: git branch [<options>] [-r | -a] [--points-at]
   or: git branch [<options>] [-r | -a] [--format]

Generic options
    -v, --verbose         show hash and subject, give twice for upstream branch
    -q, --quiet           suppress informational messages
    -t, --track[=(direct|inherit)]
                          set branch tracking configuration
    -u, --set-upstream-to <upstream>
                          change the upstream info
    --unset-upstream      unset the upstream info
    --color[=<when>]      use colored output
    -r, --remotes         act on remote-tracking branches
    --contains <commit>   print only branches that contain the commit
    --no-contains <commit>
                          print only branches that don't contain the commit
    --abbrev[=<n>]        use <n> digits to display object names

Specific git-branch actions:
    -a, --all             list both remote-tracking and local branches
    -d, --delete          delete fully merged branch
    -D                    delete branch (even if not merged)
    -m, --move            move/rename a branch and its reflog
    -M                    move/rename a branch, even if target exists
    -c, --copy            copy a branch and its reflog
    -C                    copy a branch, even if target exists
    -l, --list            list branch names
    --show-current        show current branch name
    --create-reflog       create the branch's reflog
    --edit-description    edit the description for the branch
    -f, --force           force creation, move/rename, deletion
    --merged <commit>     print only branches that are merged
    --no-merged <commit>  print only branches that are not merged
    --column[=<style>]    list branches in columns
    --sort <key>          field name to sort on
    --points-at <object>  print only branches of the object
    -i, --ignore-case     sorting and filtering are case insensitive
    --recurse-submodules  recurse through submodules
    --format <format>     format to use for the output


HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (ft/faq-page)
$ git branch -b ft/home-page-redesign
error: unknown switch `b'
usage: git branch [<options>] [-r | -a] [--merged] [--no-merged]
   or: git branch [<options>] [-f] [--recurse-submodules] <branch-name> [<start-point>]
   or: git branch [<options>] [-l] [<pattern>...]
   or: git branch [<options>] [-r] (-d | -D) <branch-name>...
   or: git branch [<options>] (-m | -M) [<old-branch>] <new-branch>
   or: git branch [<options>] (-c | -C) [<old-branch>] <new-branch>
   or: git branch [<options>] [-r | -a] [--points-at]
   or: git branch [<options>] [-r | -a] [--format]

Generic options
    -v, --verbose         show hash and subject, give twice for upstream branch
    -q, --quiet           suppress informational messages
    -t, --track[=(direct|inherit)]
                          set branch tracking configuration
    -u, --set-upstream-to <upstream>
                          change the upstream info
    --unset-upstream      unset the upstream info
    --color[=<when>]      use colored output
    -r, --remotes         act on remote-tracking branches
    --contains <commit>   print only branches that contain the commit
    --no-contains <commit>
                          print only branches that don't contain the commit
    --abbrev[=<n>]        use <n> digits to display object names

Specific git-branch actions:
    -a, --all             list both remote-tracking and local branches
    -d, --delete          delete fully merged branch
    -D                    delete branch (even if not merged)
    -m, --move            move/rename a branch and its reflog
    -M                    move/rename a branch, even if target exists
    -c, --copy            copy a branch and its reflog
    -C                    copy a branch, even if target exists
    -l, --list            list branch names
    --show-current        show current branch name
    --create-reflog       create the branch's reflog
    --edit-description    edit the description for the branch
    -f, --force           force creation, move/rename, deletion
    --merged <commit>     print only branches that are merged
    --no-merged <commit>  print only branches that are not merged
    --column[=<style>]    list branches in columns
    --sort <key>          field name to sort on
    --points-at <object>  print only branches of the object
    -i, --ignore-case     sorting and filtering are case insensitive
    --recurse-submodules  recurse through submodules
    --format <format>     format to use for the output


HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (ft/faq-page)
$ git checkout -b ft/home-page-redesign
Switched to a new branch 'ft/home-page-redesign'

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (ft/home-page-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (main)
$ git add .

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (main)
$ git commit -m "somechanges on home "
[main 32d7e21] somechanges on home
 1 file changed, 3 insertions(+), 1 deletion(-)

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (main)
$ git push 
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 309 bytes | 309.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/angep72/Gym-Git-Exercise-Solutions.git
   a44743a..32d7e21  main -> main

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (main)
$ git checkout ft/home-page-redesign
Switched to branch 'ft/home-page-redesign'

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (ft/home-page-redesign)
$ git fetch origin main
^C

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (ft/home-page-redesign)
$ git fetch origin main 
From https://github.com/angep72/Gym-Git-Exercise-Solutions
 * branch            main       -> FETCH_HEAD

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (ft/home-page-redesign)
$ git rebase ft/home-page-redesign
Current branch ft/home-page-redesign is up to date.

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (ft/home-page-redesign)
$ git rebase origin/main
^C

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (ft/home-page-redesign)
$ git rebase origin/main
Successfully rebased and updated refs/heads/ft/home-page-redesign.

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (ft/home-page-redesign)
$ git push origin your-branch-name --force
^C

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (ft/home-page-redesign)
$ git push origin ft/home-page-redesign
Enumerating objects: 16, done.
Counting objects: 100% (16/16), done.
Delta compression using up to 8 threads
Compressing objects: 100% (14/14), done.
Writing objects: 100% (14/14), 1.43 KiB | 1.43 MiB/s, done.
Total 14 (delta 8), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (8/8), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/home-page-redesign' on GitHub by visiting:
remote:      https://github.com/angep72/Gym-Git-Exercise-Solutions/pull/new/ft/home-page-redesign
remote:
To https://github.com/angep72/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/home-page-redesign -> ft/home-page-redesign

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (ft/home-page-redesign)
$ git status
On branch ft/home-page-redesign
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   home.html

no changes added to commit (use "git add" and/or "git commit -a")

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (ft/home-page-redesign)
$ git add .

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (ft/home-page-redesign)
$ git commit -m "home"
[ft/home-page-redesign b2eef76] home
 1 file changed, 1 insertion(+), 1 deletion(-)

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (ft/home-page-redesign)
$ git push 
fatal: The current branch ft/home-page-redesign has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/home-page-redesign

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (ft/home-page-redesign)
$ git push --set-upstream origin ft/home-page-redesign
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 286 bytes | 286.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/angep72/Gym-Git-Exercise-Solutions.git
   b910dcf..b2eef76  ft/home-page-redesign -> ft/home-page-redesign
branch 'ft/home-page-redesign' set up to track 'origin/ft/home-page-redesign'.

HP@DESKTOP-1CTEVNT MINGW64 ~/git-exercises (ft/home-page-redesign)
```


 