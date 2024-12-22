# Gym_Git_Exercise_Solutions

## bundle1
## exercise1
```bash

adeli@DESKTOP-SGKPF3E MINGW64 ~
$ mkdir project1

adeli@DESKTOP-SGKPF3E MINGW64 ~
$ cd project1

adeli@DESKTOP-SGKPF3E MINGW64 ~/project1
$ git init
Initialized empty Git repository in C:/Users/adeli/project1/.git/

adeli@DESKTOP-SGKPF3E MINGW64 ~/project1 (main)
$ touch index.html

adeli@DESKTOP-SGKPF3E MINGW64 ~/project1 (main)
$ nano index.html

adeli@DESKTOP-SGKPF3E MINGW64 ~/project1 (main)
$ git branch

adeli@DESKTOP-SGKPF3E MINGW64 ~/project1 (main)
$ git branch -m master

adeli@DESKTOP-SGKPF3E MINGW64 ~/project1 (master)
$ git add .
warning: in the working copy of 'index.html', LF will be replaced by CRLF the next time Git touches it

adeli@DESKTOP-SGKPF3E MINGW64 ~/project1 (master)
$ git add .

adeli@DESKTOP-SGKPF3E MINGW64 ~/project1 (master)
$ git commit -m "first commit"
[master (root-commit) e4f8c34] first commit
 1 file changed, 45 insertions(+)
 create mode 100644 index.html

adeli@DESKTOP-SGKPF3E MINGW64 ~/project1 (master)
$ git remote add origin https://github.com/adeline333/Gym_Git_Exercise_Solutions.git

adeli@DESKTOP-SGKPF3E MINGW64 ~/project1 (master)
$ git push -u origin master
fatal: unable to access 'https://github.com/adeline333/Gym_Git_Exercise_Solutions.git/': Failed to connect to github.com port 443 after 21202 ms: Could not connect to server

adeli@DESKTOP-SGKPF3E MINGW64 ~/project1 (master)
$ git push -u origin master
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 729 bytes | 729.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote:
remote: Create a pull request for 'master' on GitHub by visiting:
remote:      https://github.com/adeline333/Gym_Git_Exercise_Solutions/pull/new/master
remote:
To https://github.com/adeline333/Gym_Git_Exercise_Solutions.git
 * [new branch]      master -> master
branch 'master' set up to track 'origin/master'.

adeli@DESKTOP-SGKPF3E MINGW64 ~/project1 (master)
$ git checkout -b dev
Switched to a new branch 'dev'

adeli@DESKTOP-SGKPF3E MINGW64 ~/project1 (dev)
$ git chackout -b test
git: 'chackout' is not a git command. See 'git --help'.

The most similar command is
        checkout

adeli@DESKTOP-SGKPF3E MINGW64 ~/project1 (dev)
$ git checkout -b test
Switched to a new branch 'test'

adeli@DESKTOP-SGKPF3E MINGW64 ~/project1 (test)
$ git checkout dev
Switched to branch 'dev'

adeli@DESKTOP-SGKPF3E MINGW64 ~/project1 (dev)
$ git branch -d test
Deleted branch test (was e4f8c34).

```

## bundle 1
## exercise 2
```bash
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions> git status
On branch main
Your branch is up to date with 'origin/main'.

Untracked files:
        home.html

PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions> git add "home.html"
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   home.html

PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions> git stash save"home.html"
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions> git stash save "home.html"
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions> git status
On branch main
Your branch is up to date with 'origin/main'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        about.html

PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions> git stash save "about.html"        
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions> git status
On branch main
Your branch is up to date with 'origin/main'.
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        team.html

nothing added to commit but untracked files present (use "git add" to track)
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions> git add "team.html"
Saved working directory and index state On main: team.html
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions> git stash list
stash@{0}: On main: team.html
stash@{1}: On main: about.html
stash@{2}: On main: home.html
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions> git stash pop 1
On branch main

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   home.html

Dropped refs/stash@{1} (851729355da3d7fbd02ce7cc2ddeaee90228b94a)
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions> git commit -m "exercise 2 bundle1" 
[main 6f046d6] exercise 2 bundle1
 create mode 100644 about.html
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions> git push -u origin main
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 514 bytes | 171.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/adeline333/Gym_Git_Exercise_Solutions.git
branch 'main' set up to track 'origin/main'.
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions> git stash list
stash@{0}: On main: team.html
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions> git stash pop 0
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions> git reset --hard
HEAD is now at 6f046d6 exercise 2 bundle1
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions> git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions> 

```
## bundle 2
## exercise 1
```bash

* main
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions> git checkout ft/bundle-2
Switched to branch 'ft/bundle-2'
On branch ft/bundle-2
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        services.html

nothing added to commit but untracked files present (use "git add" to track)
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions> git add "services.html"
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions> git commit -m "added the the services.html page"
[ft/bundle-2 8577a13] added the the services.html page
 1 file changed, 10 insertions(+)
 create mode 100644 services.html
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions> git push origin ft/bundle-2       
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 424 bytes | 424.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote:      https://github.com/adeline333/Gym_Git_Exercise_Solutions/pull/new/ft/bundle-
remote:
To https://github.com/adeline333/Gym_Git_Exercise_Solutions.git
 * [new branch]      ft/bundle-2 -> ft/bundle-2
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions>

```