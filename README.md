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