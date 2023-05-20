# Gym Git Exercise Solutions

karer@DESKTOP-ALDB193 MINGW64 /e/thegym/week2 (main)
$ mkdir project

karer@DESKTOP-ALDB193 MINGW64 /e/thegym/week2 (main)
$ cd project/

karer@DESKTOP-ALDB193 MINGW64 /e/thegym/week2/project (main)
$ touch index.html

karer@DESKTOP-ALDB193 MINGW64 /e/thegym/week2/project (main)
$ nano index.html

karer@DESKTOP-ALDB193 MINGW64 /e/thegym/week2/project (main)
$ echo "# the-gym-git-basics" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/kareraolivier/the-gym-git-basics.git
git push -u origin main
Initialized empty Git repository in E:/thegym/week2/project/.git/
warning: in the working copy of 'README.md', LF will be replaced by CRLF the next time Git touches it
[master (root-commit) 9319827] first commit
 1 file changed, 1 insertion(+)
 create mode 100644 README.md

Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 232 bytes | 116.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/kareraolivier/the-gym-git-basics.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.

karer@DESKTOP-ALDB193 MINGW64 /e/thegym/week2/project (main)
$

karer@DESKTOP-ALDB193 MINGW64 /e/thegym/week2/project (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        index.html

nothing added to commit but untracked files present (use "git add" to track)

karer@DESKTOP-ALDB193 MINGW64 /e/thegym/week2/project (main)
$ git add .
warning: in the working copy of 'index.html', LF will be replaced by CRLF the next time Git touches it

karer@DESKTOP-ALDB193 MINGW64 /e/thegym/week2/project (main)
$ git commit -m "adding index file"
[main 3182bd0] adding index file
 1 file changed, 10 insertions(+)
 create mode 100644 index.html

karer@DESKTOP-ALDB193 MINGW64 /e/thegym/week2/project (main)
$ git push
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 358 bytes | 358.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/kareraolivier/the-gym-git-basics.git
   9319827..3182bd0  main -> main

karer@DESKTOP-ALDB193 MINGW64 /e/thegym/week2/project (main)
$ git cheackout -b dev
git: 'cheackout' is not a git command. See 'git --help'.

The most similar command is
        checkout

karer@DESKTOP-ALDB193 MINGW64 /e/thegym/week2/project (main)
$ git checkout -b dev
Switched to a new branch 'dev'

karer@DESKTOP-ALDB193 MINGW64 /e/thegym/week2/project (dev)
$ git checkout -b test
Switched to a new branch 'test'

karer@DESKTOP-ALDB193 MINGW64 /e/thegym/week2/project (test)
$ git checkout dev
Switched to branch 'dev'

karer@DESKTOP-ALDB193 MINGW64 /e/thegym/week2/project (dev)
$ git delete branch test
git: 'delete' is not a git command. See 'git --help'.

karer@DESKTOP-ALDB193 MINGW64 /e/thegym/week2/project (dev)
$ git branch --delete test
Deleted branch test (was 3182bd0).

karer@DESKTOP-ALDB193 MINGW64 /e/thegym/week2/project (dev)
$ nano index.html

karer@DESKTOP-ALDB193 MINGW64 /e/thegym/week2/project (dev)
$ git add .
warning: in the working copy of 'index.html', LF will be replaced by CRLF the next time Git touches it

karer@DESKTOP-ALDB193 MINGW64 /e/thegym/week2/project (dev)
$ git commit -m "test branch"
[dev db6f84f] test branch
 1 file changed, 1 insertion(+), 1 deletion(-)

karer@DESKTOP-ALDB193 MINGW64 /e/thegym/week2/project (dev)
$ git push
fatal: The current branch dev has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin dev

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


karer@DESKTOP-ALDB193 MINGW64 /e/thegym/week2/project (dev)
$ git push --set-upstream origin dev
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 365 bytes | 33.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'dev' on GitHub by visiting:
remote:      https://github.com/kareraolivier/the-gym-git-basics/pull/new/dev
remote:
To https://github.com/kareraolivier/the-gym-git-basics.git
 * [new branch]      dev -> dev
branch 'dev' set up to track 'origin/dev'.

karer@DESKTOP-ALDB193 MINGW64 /e/thegym/week2/project (dev)
$ ls
README.md  index.html

karer@DESKTOP-ALDB193 MINGW64 /e/thegym/week2/project (dev)
$ touch home.html

karer@DESKTOP-ALDB193 MINGW64 /e/thegym/week2/project (dev)
$ nano home.html

karer@DESKTOP-ALDB193 MINGW64 /e/thegym/week2/project (dev)
$ touch about.html

karer@DESKTOP-ALDB193 MINGW64 /e/thegym/week2/project (dev)
$ touch team.html

karer@DESKTOP-ALDB193 MINGW64 /e/thegym/week2/project (dev)
$ ls
README.md  about.html  home.html  index.html  team.html

karer@DESKTOP-ALDB193 MINGW64 /e/thegym/week2/project (dev)
$ nano home.html

karer@DESKTOP-ALDB193 MINGW64 /e/thegym/week2/project (dev)
$ nano about.html

karer@DESKTOP-ALDB193 MINGW64 /e/thegym/week2/project (dev)
$ nano home.html

karer@DESKTOP-ALDB193 MINGW64 /e/thegym/week2/project (dev)
$ nano about.html

karer@DESKTOP-ALDB193 MINGW64 /e/thegym/week2/project (dev)
$ nano team.html

karer@DESKTOP-ALDB193 MINGW64 /e/thegym/week2/project (dev)
$ git stash
No local changes to save

karer@DESKTOP-ALDB193 MINGW64 /e/thegym/week2/project (dev)
$ lsl
bash: lsl: command not found

karer@DESKTOP-ALDB193 MINGW64 /e/thegym/week2/project (dev)
$ ls
README.md  about.html  home.html  index.html  team.html

karer@DESKTOP-ALDB193 MINGW64 /e/thegym/week2/project (dev)
$ git status
On branch dev
Your branch is up to date with 'origin/dev'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        about.html
        home.html
        team.html

nothing added to commit but untracked files present (use "git add" to track)

karer@DESKTOP-ALDB193 MINGW64 /e/thegym/week2/project (dev)
$ git stash team.html
fatal: subcommand wasn't specified; 'push' can't be assumed due to unexpected token 'team.html'

karer@DESKTOP-ALDB193 MINGW64 /e/thegym/week2/project (dev)
$ git add home.html
warning: in the working copy of 'home.html', LF will be replaced by CRLF the next time Git touches it

karer@DESKTOP-ALDB193 MINGW64 /e/thegym/week2/project (dev)
$ git status
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   home.html

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        about.html
        team.html


karer@DESKTOP-ALDB193 MINGW64 /e/thegym/week2/project (dev)
$ git stash
Saved working directory and index state WIP on dev: db6f84f test branch

karer@DESKTOP-ALDB193 MINGW64 /e/thegym/week2/project (dev)
$ git status
On branch dev
Your branch is up to date with 'origin/dev'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        about.html
        team.html

nothing added to commit but untracked files present (use "git add" to track)

karer@DESKTOP-ALDB193 MINGW64 /e/thegym/week2/project (dev)
$ ls
README.md  about.html  index.html  team.html

karer@DESKTOP-ALDB193 MINGW64 /e/thegym/week2/project (dev)
$ git stash apply
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   home.html

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        about.html
        team.html


karer@DESKTOP-ALDB193 MINGW64 /e/thegym/week2/project (dev)
$ git add about.html
warning: in the working copy of 'about.html', LF will be replaced by CRLF the next time Git touches it

karer@DESKTOP-ALDB193 MINGW64 /e/thegym/week2/project (dev)
$ git add team.html
warning: in the working copy of 'team.html', LF will be replaced by CRLF the next time Git touches it

karer@DESKTOP-ALDB193 MINGW64 /e/thegym/week2/project (dev)
$ git status
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   home.html
        new file:   team.html


karer@DESKTOP-ALDB193 MINGW64 /e/thegym/week2/project (dev)
$ git stash
Saved working directory and index state WIP on dev: db6f84f test branch

karer@DESKTOP-ALDB193 MINGW64 /e/thegym/week2/project (dev)
$ git status
On branch dev
Your branch is up to date with 'origin/dev'.

nothing to commit, working tree clean

karer@DESKTOP-ALDB193 MINGW64 /e/thegym/week2/project (dev)
$ git stash apply
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   home.html
        new file:   team.html


karer@DESKTOP-ALDB193 MINGW64 /e/thegym/week2/project (dev)
$ git restore --staged team.html

karer@DESKTOP-ALDB193 MINGW64 /e/thegym/week2/project (dev)
$ git status
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   home.html

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        team.html


karer@DESKTOP-ALDB193 MINGW64 /e/thegym/week2/project (dev)
$ git commit -m "stash save and stash pop"
[dev f276084] stash save and stash pop
 2 files changed, 78 insertions(+)
 create mode 100644 about.html
 create mode 100644 home.html

karer@DESKTOP-ALDB193 MINGW64 /e/thegym/week2/project (dev)
$ git commit --amend --no-edit
[dev 02e2921] stash save and stash pop
 Date: Sun May 14 12:02:09 2023 +0200
 2 files changed, 78 insertions(+)
 create mode 100644 about.html
 create mode 100644 home.html

karer@DESKTOP-ALDB193 MINGW64 /e/thegym/week2/project (dev)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 677 bytes | 677.00 KiB/s, done.
Total 4 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), done.
To https://github.com/kareraolivier/the-gym-git-basics.git
   db6f84f..02e2921  dev -> dev

karer@DESKTOP-ALDB193 MINGW64 /e/thegym/week2/project (dev)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

karer@DESKTOP-ALDB193 MINGW64 /e/thegym/week2/project (main)
$ git checkout -b ft/bundle-2
Switched to a new branch 'ft/bundle-2'

karer@DESKTOP-ALDB193 MINGW64 /e/thegym/week2/project (ft/bundle-2)
$ touch service.html

karer@DESKTOP-ALDB193 MINGW64 /e/thegym/week2/project (ft/bundle-2)
$ nano service.html

karer@DESKTOP-ALDB193 MINGW64 /e/thegym/week2/project (ft/bundle-2)
$ git add .
warning: in the working copy of 'service.html', LF will be replaced by CRLF the next time Git touches it

karer@DESKTOP-ALDB193 MINGW64 /e/thegym/week2/project (ft/bundle-2)
$ git commit -m "service"
[ft/bundle-2 311361e] service
 2 files changed, 53 insertions(+)
 create mode 100644 service.html
 create mode 100644 team.html

karer@DESKTOP-ALDB193 MINGW64 /e/thegym/week2/project (ft/bundle-2)
$ git push
fatal: The current branch ft/bundle-2 has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/bundle-2

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


karer@DESKTOP-ALDB193 MINGW64 /e/thegym/week2/project (ft/bundle-2)
$ ^C

karer@DESKTOP-ALDB193 MINGW64 /e/thegym/week2/project (ft/bundle-2)
$ git push --set-upstream origin ft/bundle-2
Enumerating objects: 5, done.
  
  
  week 3
  
E:\thegym\week2\project>git branch
dev

- ft/bundle-2
  main

E:\thegym\week2\project>git checkout -b ft/service-redesign
Switched to a new branch 'ft/service-redesign'

E:\thegym\week2\project>git branch
dev
ft/bundle-2

- ft/service-redesign
  main

  karer@DESKTOP-ALDB193 MINGW64 /e/thegym/week2/project (ft/service-redesign)
  $ nanp service.html
  bash: nanp: command not found

karer@DESKTOP-ALDB193 MINGW64 /e/thegym/week2/project (ft/service-redesign)
$ nano service.html

Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 790 bytes | 790.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote:      https://github.com/kareraolivier/the-gym-git-basics/pull/new/ft/bundle-2
remote:
To https://github.com/kareraolivier/the-gym-git-basics.git
 * [new branch]      ft/bundle-2 -> ft/bundle-2
branch 'ft/bundle-2' set up to track 'origin/ft/bundle-2'.

