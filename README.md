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

## bundle 2
## exercise 2
```bash
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions-1> git branch
* main
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions-1> git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
no changes added to commit (use "git add" and/or "git commit -a")
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions-1> git commit -m "solutio
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions-1> git add .
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions-1> git commit -m "solutioPS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions-1> git checkout main
Already on 'main'                                                               n
Your branch is up to date with 'origin/main'.
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions-1> git pull origin main
From https://github.com/adeline333/Gym_Git_Exercise_Solutions
 * branch            main       -> FETCH_HEAD
Already up to date.
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions-1> git branch ft/service-redesign
On branch main
Your branch is up to date with 'origin/main'.

  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   services.html

no changes added to commit (use "git add" and/or "git commit -a")
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions-1> git add "services.html"
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions-1> git commit -m "modifiePS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions-1> git checkout main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions-1> git pull origin main  vice-redesign
From https://github.com/adeline333/Gym_Git_Exercise_Solutions
 * branch            main       -> FETCH_HEAD
Already up to date.
```bash
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions-1> git checkout ft/servict/service-redesign* ft/service-redesign
  main
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions-1> git status
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   services.html

no changes added to commit (use "git add" and/or "git commit -a")
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions-1> git add .
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions-1> git commit -m "added new content to the services page"
 1 file changed, 1 insertion(+)
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions-1> git push origin ft/service-redesign
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Writing objects: 100% (3/3), 376 bytes | 376.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/adeline333/Gym_Git_Exercise_Solutions.git
   c96aa8d..6ffdca5  ft/service-redesign -> ft/service-redesign
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions-1> git checkout main     
Switched to branch 'main'
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions-1> git branch
On branch main
Your branch is ahead of 'origin/main' by 1 commit.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   services.html

no changes added to commit (use "git add" and/or "git commit -a")
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions-1> git add .
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions-1> git commit -m "updated the services page iwth conflicting changes"
 1 file changed, 2 insertions(+), 1 deletion(-)
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 4 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 758 bytes | 189.00 KiB/s, done.
Total 6 (delta 3), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (3/3), completed with 1 local object.
To https://github.com/adeline333/Gym_Git_Exercise_Solutions.git
   c96aa8d..3538380  main -> main
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions-1> git checkout ft/service-redesign
Switched to branch 'ft/service-redesign'
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions-1> git diff main
index 4cfccaa..dd80e5f 100644
--- a/services.html
+++ b/services.html
 <body>
     <h1>Our Services</h1>
     <p>We offer a variety of services tailored to your needs.</p>
-    <p> created a new branch for redesigning"now adding another"</p>
+    <p>added the changes to the page accorf=ding to exercise 2 bundle 2</p>    
 </body>
 </html>
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions-1> git merge main        
Auto-merging services.html
CONFLICT (content): Merge conflict in services.html
Automatic merge failed; fix conflicts and then commit the result.
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions-1> git merge main        
error: Merging is not possible because you have unmerged files.
hint: Fix them up in the work tree, and then use 'git add/rm <file>'
On branch ft/service-redesign
  (fix conflicts and run "git commit")
  (use "git merge --abort" to abort the merge)

  (use "git add <file>..." to mark resolution)
        both modified:   services.html

no changes added to commit (use "git add" and/or "git commit -a")
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions-1> git add .
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions-1> git commit -m "resolved the conflicts"
[ft/service-redesign 322effb] resolved the conflicts
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions-1> git status
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions-1> git push origin ft/service-redesign
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 386 bytes | 386.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/adeline333/Gym_Git_Exercise_Solutions.git
   6ffdca5..322effb  ft/service-redesign -> ft/service-redesign
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions-1>
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions-1> git merge main
Already up to date.
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions-1>
```
## bundle 3
## exercise 1
```bash
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions> git status
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions> git add .
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions> git checkout main   cise 2 bundle 2 solution"
Already on 'main'
Your branch is up to date with 'origin/main'. 
```                             n
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions> git pull origin maiFrom https://github.com/adeline333/Gym_Git_Exercise_Solutions
Already up to date.
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions> git branch ft/team-page
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions> git ckeckout ft/team-page
git: 'ckeckout' is not a git command. See 'git --help'.                     

m-page
Switched to branch 'ft/team-page'
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions> git status
On branch ft/team-page
  (use "git add <file>..." to include in what will be committed)
        team.html

nothing added to commit but untracked files present (use "git add" to track)
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions> git add team.html  
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions> git commit -m "added the team pag" 
[ft/team-page b593462] added the team pag
 1 file changed, 11 insertions(+)
 create mode 100644 team.html
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions> git push origin  ft/team-page     
Enumerating objects: 4, done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
remote: Resolving deltas: 100% (1/1), completed with 1 local object.       
remote:
remote: Create a pull request for 'ft/team-page' on GitHub by visiting:    
remote:      https://github.com/adeline333/Gym_Git_Exercise_Solutions/pull/new/ft/team-page
remote:
To https://github.com/adeline333/Gym_Git_Exercise_Solutions.git
 * [new branch]      ft/team-page -> ft/team-page
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions> git checkout main  
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions> git pull origin mairemote: Counting objects: 100% (4/4), done.
remote: Compressing objects: 100% (2/2), done.
Unpacking objects: 100% (2/2), 979 bytes | 65.00 KiB/s, done.
 * branch            main       -> FETCH_HEAD
   33f36d0..ae34775  main       -> origin/main
Updating 33f36d0..ae34775
Fast-forward
 services.html | 6 ++++++
 1 file changed, 6 insertions(+)
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions> git checkout -b ft/contact-page
Switched to a new branch 'ft/contact-page'
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions> git checkout ft/team-page
Switched to branch 'ft/team-page'
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions> git log
Author: Adeline Tuyizere <adelinetuyizere333@gmail.com>
Date:   Mon Dec 23 11:52:39 2024 +0200
    added the team pag

commit 33f36d00f0193474ccb652626e9f1f9cb04e9434
Author: Adeline Tuyizere <adelinetuyizere333@gmail.com>
Date:   Mon Dec 23 11:37:02 2024 +0200

     exercise 2 bundle 2 solution

PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions> git checkout ft/contact-page
Switched to branch 'ft/contact-page'
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions> git cherry-pick 33f36d00f0193474ccb652626e9f1f9cb04e9434
You are currently cherry-picking commit 33f36d0.
  (all conflicts fixed: run "git cherry-pick --continue")
  (use "git cherry-pick --skip" to skip this patch)
  (use "git cherry-pick --abort" to cancel the cherry-pick operation)      

nothing to commit, working tree clean
The previous cherry-pick is now empty, possibly due to conflict resolution.If you wish to commit it anyway, use:

    git commit --allow-empty

Otherwise, please use 'git cherry-pick --skip'
  (use "git cherry-pick --skip" to skip this patch)
  (use "git cherry-pick --abort" to cancel the cherry-pick operation)      

Untracked files:

nothing added to commit but untracked files present (use "git add" to track)
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions> git add contact.html
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions> git commit -m "added the contact page"
[ft/contact-page b30aeb0] added the contact page
 Date: Mon Dec 23 11:37:02 2024 +0200
 1 file changed, 11 insertions(+)
 create mode 100644 contact.html
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions> git push origin ft/contact-page
Enumerating objects: 4, done.
Compressing objects: 100% (3/3), done.
remote: Resolving deltas: 100% (1/1), completed with 1 local object.       
remote: Create a pull request for 'ft/contact-page' on GitHub by visiting: 
remote:      https://github.com/adeline333/Gym_Git_Exercise_Solutions/pull/new/ft/contact-page
remote:
To https://github.com/adeline333/Gym_Git_Exercise_Solutions.git
 * [new branch]      ft/contact-page -> ft/contact-page
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions> git checkout ft/confaq-page
Switched to a new branch 'ft/faq-page'
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions> git status
On branch ft/faq-page
  (use "git add <file>..." to include in what will be committed)
        faq.html

nothing added to commit but untracked files present (use "git add" to track)
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions> git add faq.html   
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions> git commit -m "added initial changes to faq page"
[ft/faq-page 5d5b55b] added initial changes to faq page
 1 file changed, 11 insertions(+)
 create mode 100644 faq.html
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions> git push origin ft/faq-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 450 bytes | 225.00 KiB/s, done.
remote: Resolving deltas: 100% (1/1), completed with 1 local object.       
remote:
new/ft/faq-page
remote:
To https://github.com/adeline333/Gym_Git_Exercise_Solutions.git
 * [new branch]      ft/faq-page -> ft/faq-page
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions> git checkout ft/team-page
Switched to branch 'ft/team-page'
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions> git revert 33f36d00f0193474ccb652626e9f1f9cb04e9434
[ft/team-page f71ce66] Revert " exercise 2 bundle 2 solution"
 1 file changed, 1 insertion(+), 142 deletions(-)
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions> git push origin ft/team-page
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 367 bytes | 26.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/adeline333/Gym_Git_Exercise_Solutions.git
   b593462..f71ce66  ft/team-page -> ft/team-page
PS C:\Users\adeli\Downloads\Gym_Git_Exercise_Solutions>
```