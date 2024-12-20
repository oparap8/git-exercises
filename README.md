# Git exercise projects

# Bundle 1 Exercise 1
```bash
HP@UDO MINGW64 ~/Documents/vs code/theGym/Git exercise solution
$ git init
Initialized empty Git repository in C:/Users/HP/Documents/vs code/theGym/Git exercise solution/.git/

HP@UDO MINGW64 ~/Documents/vs code/theGym/Git exercise solution (master)
$ git branch -M main

HP@UDO MINGW64 ~/Documents/vs code/theGym/Git exercise solution (main)
$ git status
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        README.md

nothing added to commit but untracked files present (use "git add" to track)

HP@UDO MINGW64 ~/Documents/vs code/theGym/Git exercise solution (main)
$ git add README.md

HP@UDO MINGW64 ~/Documents/vs code/theGym/Git exercise solution (main)
$ git commit -m "init project"
[main (root-commit) 6765996] init project
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 README.md

HP@UDO MINGW64 ~/Documents/vs code/theGym/Git exercise solution (main)
$ git remote add origin https://github.com/oparap8/git-exercises.git

HP@UDO MINGW64 ~/Documents/vs code/theGym/Git exercise solution (main)
$ git status
On branch main
nothing to commit, working tree clean

HP@UDO MINGW64 ~/Documents/vs code/theGym/Git exercise solution (main)
$ git push
fatal: The current branch main has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin main

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


HP@UDO MINGW64 ~/Documents/vs code/theGym/Git exercise solution (main)
$ git push --set-upstream origin main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 213 bytes | 53.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/oparap8/git-exercises.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.

HP@UDO MINGW64 ~/Documents/vs code/theGym/Git exercise solution (main)
$ git push
Everything up-to-date

HP@UDO MINGW64 ~/Documents/vs code/theGym/Git exercise solution (main)
$ git checkout -b dev
Switched to a new branch 'dev'

HP@UDO MINGW64 ~/Documents/vs code/theGym/Git exercise solution (dev)
$ git push
fatal: The current branch dev has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin dev

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


HP@UDO MINGW64 ~/Documents/vs code/theGym/Git exercise solution (dev)
$ git push --set-upstream origin dev
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote: 
remote: Create a pull request for 'dev' on GitHub by visiting:
remote:      https://github.com/oparap8/git-exercises/pull/new/dev
remote:
To https://github.com/oparap8/git-exercises.git
 * [new branch]      dev -> dev
branch 'dev' set up to track 'origin/dev'.

HP@UDO MINGW64 ~/Documents/vs code/theGym/Git exercise solution (dev)
$ git checkout -b test
Switched to a new branch 'test'

HP@UDO MINGW64 ~/Documents/vs code/theGym/Git exercise solution (test)
$ git push origin test
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote: 
remote: Create a pull request for 'test' on GitHub by visiting:
remote:      https://github.com/oparap8/git-exercises/pull/new/test
remote:
To https://github.com/oparap8/git-exercises.git
 * [new branch]      test -> test

HP@UDO MINGW64 ~/Documents/vs code/theGym/Git exercise solution (test)
$ git checkout dev
Switched to branch 'dev'
Your branch is up to date with 'origin/dev'.

HP@UDO MINGW64 ~/Documents/vs code/theGym/Git exercise solution (dev)
$ git branch -d test
Deleted branch test (was 6765996).

HP@UDO MINGW64 ~/Documents/vs code/theGym/Git exercise solution (dev)
$ git push origin --delete test
To https://github.com/oparap8/git-exercises.git
 - [deleted]         test
```

# Bundle 1 Exercise 2

```bash

HP@UDO MINGW64 ~/Documents/vs code/theGym/Git exercise solution (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        home.html

nothing added to commit but untracked files present (use "git add" to track)

HP@UDO MINGW64 ~/Documents/vs code/theGym/Git exercise solution (main)
$ git add home.html

HP@UDO MINGW64 ~/Documents/vs code/theGym/Git exercise solution (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   home.html


HP@UDO MINGW64 ~/Documents/vs code/theGym/Git exercise solution (main)
$ git stash
Saved working directory and index state WIP on main: e3b11fd README for Bundle 1 Exercise 1

HP@UDO MINGW64 ~/Documents/vs code/theGym/Git exercise solution (main)
$ git stash list
stash@{0}: WIP on main: e3b11fd README for Bundle 1 Exercise 1

HP@UDO MINGW64 ~/Documents/vs code/theGym/Git exercise solution (main)
$ git add about.html

HP@UDO MINGW64 ~/Documents/vs code/theGym/Git exercise solution (main)
$ git stash
Saved working directory and index state WIP on main: e3b11fd README for Bundle 1 Exercise 1

HP@UDO MINGW64 ~/Documents/vs code/theGym/Git exercise solution (main)
$ git stash list
stash@{0}: WIP on main: e3b11fd README for Bundle 1 Exercise 1
stash@{1}: WIP on main: e3b11fd README for Bundle 1 Exercise 1

HP@UDO MINGW64 ~/Documents/vs code/theGym/Git exercise solution (main)
$ git add team.html

HP@UDO MINGW64 ~/Documents/vs code/theGym/Git exercise solution (main)
$ git stash
Saved working directory and index state WIP on main: e3b11fd README for Bundle 1 Exercise 1

HP@UDO MINGW64 ~/Documents/vs code/theGym/Git exercise solution (main)
$ git stash lish
fatal: subcommand wasn't specified; 'push' can't be assumed due to unexpected token 'lish'

HP@UDO MINGW64 ~/Documents/vs code/theGym/Git exercise solution (main)
$ git stash list
stash@{0}: WIP on main: e3b11fd README for Bundle 1 Exercise 1
stash@{1}: WIP on main: e3b11fd README for Bundle 1 Exercise 1
stash@{2}: WIP on main: e3b11fd README for Bundle 1 Exercise 1

HP@UDO MINGW64 ~/Documents/vs code/theGym/Git exercise solution (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean

HP@UDO MINGW64 ~/Documents/vs code/theGym/Git exercise solution (main)
$ git stash pop stash@{1}
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

Dropped stash@{1} (cd64197c3519d127b710b4d1242eab806ecd8d14)

HP@UDO MINGW64 ~/Documents/vs code/theGym/Git exercise solution (main)
$ git stash pop stash@{1}
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   home.html

Dropped stash@{1} (9d536391615a06be7781afbf20f7ca78a2780eae)

HP@UDO MINGW64 ~/Documents/vs code/theGym/Git exercise solution (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   home.html


HP@UDO MINGW64 ~/Documents/vs code/theGym/Git exercise solution (main)
$ git commit -m "setup the home and about page"
[main 039b94b] setup the home and about page
 2 files changed, 11 insertions(+)
 create mode 100644 about.html
 create mode 100644 home.html

HP@UDO MINGW64 ~/Documents/vs code/theGym/Git exercise solution (main)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (4/4), 502 bytes | 502.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/oparap8/git-exercises.git
   e3b11fd..039b94b  main -> main

HP@UDO MINGW64 ~/Documents/vs code/theGym/Git exercise solution (main)
$ git stash pop stash@{1}
fatal: log for 'stash' only has 1 entries

HP@UDO MINGW64 ~/Documents/vs code/theGym/Git exercise solution (main)
$ git stash pop stash@{0}
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

Dropped stash@{0} (13a8edd8ef435bb5abff7344504e26d7abcc77be)

HP@UDO MINGW64 ~/Documents/vs code/theGym/Git exercise solution (main)
$ git reset --hard
HEAD is now at 039b94b setup the home and about page
```
# Bundle 2 Exercise 1
```bash

HP@UDO MINGW64 ~/Documents/vs code/theGym/Git exercise solution (main)
$ git checkout -b ft/bundle-2
Switched to a new branch 'ft/bundle-2'

HP@UDO MINGW64 ~/Documents/vs code/theGym/Git exercise solution (ft/bundle-2)
$ git status
On branch ft/bundle-2
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        service.html

nothing added to commit but untracked files present (use "git add" to track)

HP@UDO MINGW64 ~/Documents/vs code/theGym/Git exercise solution (ft/bundle-2)
$ git add service.html

HP@UDO MINGW64 ~/Documents/vs code/theGym/Git exercise solution (ft/bundle-2)
$ git commit -m "create service page"
[ft/bundle-2 486dd91] create service page
 1 file changed, 11 insertions(+)
 create mode 100644 service.html

HP@UDO MINGW64 ~/Documents/vs code/theGym/Git exercise solution (ft/bundle-2)
$ git push
fatal: The current branch ft/bundle-2 has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/bundle-2

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


HP@UDO MINGW64 ~/Documents/vs code/theGym/Git exercise solution (ft/bundle-2)
$ git push --set-upstream origin ft/bundle-2
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 453 bytes | 453.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote:      https://github.com/oparap8/git-exercises/pull/new/ft/bundle-2
remote:
To https://github.com/oparap8/git-exercises.git
 * [new branch]      ft/bundle-2 -> ft/bundle-2
branch 'ft/bundle-2' set up to track 'origin/ft/bundle-2'.
```
# Bundle 2 Exercise 2
```bash

HP@UDO MINGW64 ~/Documents/vs code/theGym/Git exercise solution (main)
$ git checkout -b ft/service-redesign
Switched to a new branch 'ft/service-redesign'

HP@UDO MINGW64 ~/Documents/vs code/theGym/Git exercise solution (ft/service-redesign)
$ git add --all

HP@UDO MINGW64 ~/Documents/vs code/theGym/Git exercise solution (ft/service-redesign)
$ git commit -m "feat: add service list"
[ft/service-redesign ed8d939] feat: add service list
 1 file changed, 11 insertions(+)
 create mode 100644 service.html

HP@UDO MINGW64 ~/Documents/vs code/theGym/Git exercise solution (ft/service-redesign)
$ git push
fatal: The current branch ft/service-redesign has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/service-redesign

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


HP@UDO MINGW64 ~/Documents/vs code/theGym/Git exercise solution (ft/service-redesign)
$ git push --set-upstream origin ft/service-redesign
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 455 bytes | 455.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/service-redesign' on GitHub by visiting:
remote:      https://github.com/oparap8/git-exercises/pull/new/ft/service-redesign
remote:
To https://github.com/oparap8/git-exercises.git
 * [new branch]      ft/service-redesign -> ft/service-redesign
branch 'ft/service-redesign' set up to track 'origin/ft/service-redesign'.

HP@UDO MINGW64 ~/Documents/vs code/theGym/Git exercise solution (ft/service-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

HP@UDO MINGW64 ~/Documents/vs code/theGym/Git exercise solution (main)
$ git checkout ft/service-redesign
Switched to branch 'ft/service-redesign'
Your branch is up to date with 'origin/ft/service-redesign'.

HP@UDO MINGW64 ~/Documents/vs code/theGym/Git exercise solution (ft/service-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

HP@UDO MINGW64 ~/Documents/vs code/theGym/Git exercise solution (main)
$ git add service.html
fatal: pathspec 'service.html' did not match any files

HP@UDO MINGW64 ~/Documents/vs code/theGym/Git exercise solution (main)
$ git add service.html

HP@UDO MINGW64 ~/Documents/vs code/theGym/Git exercise solution (main)
$ git commit -m "feat: add old services"
[main 619f051] feat: add old services
 1 file changed, 17 insertions(+)
 create mode 100644 service.html

HP@UDO MINGW64 ~/Documents/vs code/theGym/Git exercise solution (main)
$ git push
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 487 bytes | 487.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/oparap8/git-exercises.git
   f91a649..619f051  main -> main

HP@UDO MINGW64 ~/Documents/vs code/theGym/Git exercise solution (main)
$ git checkout ft/service-redesign
Switched to branch 'ft/service-redesign'
Your branch is up to date with 'origin/ft/service-redesign'.

HP@UDO MINGW64 ~/Documents/vs code/theGym/Git exercise solution (ft/service-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

HP@UDO MINGW64 ~/Documents/vs code/theGym/Git exercise solution (main)
$ git checkout ft/service-redesign
Switched to branch 'ft/service-redesign'
Your branch is up to date with 'origin/ft/service-redesign'.

HP@UDO MINGW64 ~/Documents/vs code/theGym/Git exercise solution (ft/service-redesign)
$ git add --all

HP@UDO MINGW64 ~/Documents/vs code/theGym/Git exercise solution (ft/service-redesign)
$ git commit -m "feat: redesign"
[ft/service-redesign 7302344] feat: redesign
 1 file changed, 7 insertions(+), 1 deletion(-)

HP@UDO MINGW64 ~/Documents/vs code/theGym/Git exercise solution (ft/service-redesign)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 353 bytes | 353.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/oparap8/git-exercises.git
   ed8d939..7302344  ft/service-redesign -> ft/service-redesign

HP@UDO MINGW64 ~/Documents/vs code/theGym/Git exercise solution (ft/service-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

HP@UDO MINGW64 ~/Documents/vs code/theGym/Git exercise solution (main)
$ git checkout ft/service-redesign
Switched to branch 'ft/service-redesign'
Your branch is up to date with 'origin/ft/service-redesign'.

HP@UDO MINGW64 ~/Documents/vs code/theGym/Git exercise solution (ft/service-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

HP@UDO MINGW64 ~/Documents/vs code/theGym/Git exercise solution (main)
$ git checkout ft/service-redesign
Switched to branch 'ft/service-redesign'
Your branch is up to date with 'origin/ft/service-redesign'.

HP@UDO MINGW64 ~/Documents/vs code/theGym/Git exercise solution (ft/service-redesign)
$ git merge main
Auto-merging service.html
CONFLICT (add/add): Merge conflict in service.html
Automatic merge failed; fix conflicts and then commit the result.

HP@UDO MINGW64 ~/Documents/vs code/theGym/Git exercise solution (ft/service-redesign|MERGING)
$ git add service.html

HP@UDO MINGW64 ~/Documents/vs code/theGym/Git exercise solution (ft/service-redesign|MERGING)
$ git commit 
[ft/service-redesign 2aefa01] Merge branch 'main' into ft/service-redesign
```