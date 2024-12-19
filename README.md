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




```bash