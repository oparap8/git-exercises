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