# Git Exercises

## Bundle 1
### Exercise 1
```bash
Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle1 (master)
$ git init
Reinitialized existing Git repository in C:/Users/Amalitech/Desktop/AmaliTech/gitExercisesProject/bundle1/.git/

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle1 (master)
$ git branch -m main

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle1 (main)
$ git status
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   README.md
        new file:   index.html


Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle1 (main)
$ git add .

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle1 (main)
$ git status
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   README.md
        new file:   index.html


Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle1 (main)
$  git commit -m "First commit on git exercise bundle one"
[main (root-commit) 3d2245d] First commit on git exercise bundle one
 2 files changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 README.md
 create mode 100644 index.html

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle1 (main)
$ git remote add origin https://github.com/umbereye27/GitExerciseSolutions.git

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle1 (main)
$ git push
fatal: The current branch main has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin main

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle1 (main)
$   git push --set-upstream origin main
Enumerating objects: 3, done.       
Counting objects: 100% (3/3), done. 
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 244 bytes | 244.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/umbereye27/GitExerciseSolutions.git
 * [new branch]      main -> main   
branch 'main' set up to track 'origin/main'.

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle1 (main)
$ git checkout -b dev
Switched to a new branch 'dev'

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle1 (dev)
$ git push 
fatal: The current branch dev has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin dev

To have this happen automatically for branches without a tracking       
upstream, see 'push.autoSetupRemote' in 'git help config'.


Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle1 (dev)
$   git push --set-upstream origin dev
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote: 
remote: Create a pull request for 'dev' on GitHub by visiting:
remote:      https://github.com/umbereye27/GitExerciseSolutions/pull/new/dev
remote:
To https://github.com/umbereye27/GitExerciseSolutions.git
 * [new branch]      dev -> dev     
branch 'dev' set up to track 'origin/dev'.

Switched to a new branch 'test'

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle1 (test)
$ git checkout dev
M       index.html
Switched to branch 'dev'
Your branch is up to date with 'origin/dev'.

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle1 (dev)
$ git branch -d test
Deleted branch test (was 3d2245d).

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle1 (dev)
$
```



### Exercise 2

```bash
Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle1 (dev)
$ git add home.html

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle1 (dev)
$ git status
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   home.html       

Changes not staged for commit:      
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory) 
        modified:   README.md       
        modified:   index.html      


Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle1 (dev)
$ git stash
Saved working directory and index state WIP on dev: 3d2245d First commit on git exercise bundle one

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle1 (dev)
$ git add about.html

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle1 (dev)
$ git stash
Saved working directory and index state WIP on dev: 3d2245d First commit on git exercise bundle one

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle1 (dev)
$ git stash lish
fatal: subcommand wasn't specified; 'push' can't be assumed due to unexpected token 'lish'

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle1 (dev)
$ git stash list
stash@{0}: WIP on dev: 3d2245d First commit on git exercise bundle one  
stash@{1}: WIP on dev: 3d2245d First commit on git exercise bundle one  

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle1 (dev)
$ git add team.html

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle1 (dev)
$ git stash
Saved working directory and index state WIP on dev: 3d2245d First commit on git exercise bundle one

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle1 (dev)
$ git stash list
stash@{0}: WIP on dev: 3d2245d First commit on git exercise bundle one  
stash@{1}: WIP on dev: 3d2245d First commit on git exercise bundle one  
stash@{2}: WIP on dev: 3d2245d First commit on git exercise bundle one  

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle1 (dev)
$ git stash pop stash@{1}
error: The following untracked working tree files would be overwritten by merge:
        about.html
Please move or remove them before you merge.
Aborting
On branch dev
Your branch is up to date with 'origin/dev'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)        
        about.html
        team.html

nothing added to commit but untracked files present (use "git add" to track)
Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle1 (dev)
$ git stash list
stash@{0}: WIP on dev: 3d2245d First commit on git exercise bundle one
stash@{1}: WIP on dev: 3d2245d First commit on git exercise bundle one
stash@{2}: WIP on dev: 3d2245d First commit on git exercise bundle one

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle1 (dev)
$ git stash list
stash@{0}: WIP on dev: 3d2245d First commit on git exercise bundle one
stash@{1}: WIP on dev: 3d2245d First commit on git exercise bundle one
stash@{2}: WIP on dev: 3d2245d First commit on git exercise bundle one

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle1 (dev)
$ git status
On branch dev
Your branch is up to date with 'origin/dev'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        about.html
        team.html

nothing added to commit but untracked files present (use "git add" to track)

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle1 (dev)
$ git add team.html

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle1 (dev)
$ git status
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        about.html


Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle1 (dev)
$ git stash
Saved working directory and index state WIP on dev: 3d2245d First commit on git exercise bundle one

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle1 (dev)
$ git stash list
stash@{0}: WIP on dev: 3d2245d First commit on git exercise bundle one
stash@{1}: WIP on dev: 3d2245d First commit on git exercise bundle one
stash@{2}: WIP on dev: 3d2245d First commit on git exercise bundle one
stash@{3}: WIP on dev: 3d2245d First commit on git exercise bundle one

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle1 (dev)
$ git stash show stash@{0}
 team.html | 11 +++++++++++
 1 file changed, 11 insertions(+)

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle1 (dev)
$ git stash show stash@{1}
 team.html | 0
 1 file changed, 0 insertions(+), 0 deletions(-)

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle1 (dev)
$ git stash show stash@{2}
 about.html | 0
 1 file changed, 0 insertions(+), 0 deletions(-)

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle1 (dev)
$ git stash show stash@{3}
 README.md  | 113 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 home.html  |  11 ++++++
 index.html |  11 ++++++
 3 files changed, 135 insertions(+)

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle1 (dev)
$ git stash pop stash@{3}
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   home.html

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md       
        modified:   index.html      

Untracked files:
  (use "git add <file>..." to include in what will be committed)        
        about.html

Dropped stash@{3} (cd6e51a1b9efb9e498f68017ee0388f85da1d459)

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle1 (dev)
$ git commit -m "Adding home and about pages"
[dev 55ef154] Adding home and about pages
 1 file changed, 11 insertions(+)   
 create mode 100644 home.html       

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle1 (dev)
$ git reset --soft HEAD~1
git staus
git: 'staus' is not a git command. See 'git --help'.

The most similar command is
        status

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle1 (dev)
$ git status
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   home.html       

Changes not staged for commit:      
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory) 
        modified:   README.md       
        modified:   index.html      

Untracked files:
  (use "git add <file>..." to include in what will be committed)        
        about.html
        team.html


Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle1 (dev)
$ git add .

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle1 (dev)
$ git commit -m "Adding home and about pages"
[dev c0c4805] Adding home and about pages
 5 files changed, 157 insertions(+) 
 create mode 100644 about.html      
 create mode 100644 home.html       
 create mode 100644 team.html       

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle1 (dev)
$ git stash list
stash@{0}: WIP on dev: 3d2245d First commit on git exercise bundle one  
stash@{1}: WIP on dev: 3d2245d First commit on git exercise bundle one  
stash@{2}: WIP on dev: 3d2245d First commit on git exercise bundle one  

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle1 (dev)
$ git stash show stash@{0}
 team.html | 11 +++++++++++
 1 file changed, 11 insertions(+)   

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle1 (dev)
$ git push
Enumerating objects: 10, done.
Counting objects: 100% (9/9), done. 
Delta compression using up to 8 threads
Compressing objects: 100% (7/7), done.
Writing objects: 100% (7/7), 1.65 KiB | 423.00 KiB/s, done.
Total 7 (delta 3), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (3/3), done.
To https://github.com/umbereye27/GitExerciseSolutions.git
   3d2245d..c0c4805  dev -> dev     

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle1 (dev)
$ git stash pop stash@{0}
On branch dev
Your branch is up to date with 'origin/dev'.

nothing to commit, working tree clean
Dropped stash@{0} (ffb6a63d5ba829adf84c5963a6165841698fa318)

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle1 (dev)
$ git stash show 
 team.html | 0
 1 file changed, 0 insertions(+), 0 deletions(-)

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle1 (dev)
$ git status
On branch dev
Your branch is up to date with 'origin/dev'.

Changes not staged for commit:      
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory) 
        modified:   team.html       

no changes added to commit (use "git add" and/or "git commit -a")       

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle1 (dev)
$ git stash
Saved working directory and index state WIP on dev: c0c4805 Adding home and about pages

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle1 (dev)
$ git stash list
stash@{0}: WIP on dev: c0c4805 Adding home and about pages
stash@{1}: WIP on dev: 3d2245d First commit on git exercise bundle one  
stash@{2}: WIP on dev: 3d2245d First commit on git exercise bundle one  

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle1 (dev)
$ git stash show stash@{0}
 team.html | 11 -----------
 1 file changed, 11 deletions(-)

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle1 (dev)
$ git reset --hard
HEAD is now at c0c4805 Adding home and about pages

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle1 (dev)
$ git status
On branch dev
Your branch is up to date with 'origin/dev'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   team.html

no changes added to commit (use "git add" and/or "git commit -a")

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle1 (dev)
$ git stash
Saved working directory and index state WIP on dev: c0c4805 Adding home and about pages

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle1 (dev)
$ git reset --hard
HEAD is now at c0c4805 Adding home and about pages


no changes added to commit (use "git add" and/or "git commit -a")

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle1 (dev)
$ git stash
Saved working directory and index state WIP on dev: c0c4805 Adding home and about pages

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle1 (dev)
$ git reset --hard
HEAD is now at c0c4805 Adding home and about pages

Saved working directory and index state WIP on dev: c0c4805 Adding home and about pages

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle1 (dev)
$ git reset --hard
HEAD is now at c0c4805 Adding home and about pages

HEAD is now at c0c4805 Adding home and about pages

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle1 (dev)
$ 
```
## Bundle 2

### Exercise 1

```bash
Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (main)
$ git checkout -b ft/bundle-2 
Switched to a new branch 'ft/bundle-2'

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/bundle-2)
$ git add services.html
fatal: pathspec 'services.html' did not match any files

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/bundle-2)
$ git add .

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/bundle-2)
$ git status
On branch ft/bundle-2
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   service.html    


Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/bundle-2)
$ git commit -m "Added services.html page"
[ft/bundle-2 36718b6] Added services.html page
 1 file changed, 11 insertions(+)   
 create mode 100644 service.html    

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/bundle-2)
$ git push
fatal: The current branch ft/bundle-2 has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/bundle-2

To have this happen automatically for branches without a tracking       
upstream, see 'push.autoSetupRemote' in 'git help config'.


Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/bundle-2)
$  git push --set-upstream origin ft/bundle-2
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done. 
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 450 bytes | 450.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote: 
reye27/Bundle-2/pull/new/ft/bundle-
remote:
To https://github.com/umbereye27/Bundle-2.git
 * [new branch]      ft/bundle-2 -> ft/bundle-2
branch 'ft/bundle-2' set up to track 'origin/ft/bundle-2'.

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/bundle-2)     
```

### Exercise 2
```bash
Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (main)
$ git checkout  ft/service-redesign 
Switched to branch 'ft/service-redesign'

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/service-redesign)    
$ git status
On branch ft/service-redesign
Untracked files:
  (use "git add <file>..." to include in what will be committed)        
        service.html

nothing added to commit but untracked files present (use "git add" to track)

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/service-redesign)    
$ git add .

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/service-redesign)    
$ git commit -m "Updated services.html with additional content"
[ft/service-redesign 4ed0e43] Updated services.html with additional content
 1 file changed, 12 insertions(+)   
 create mode 100644 service.html    

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/service-redesign)    
$ git push origin ft/service-redesign
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done. 
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 508 bytes | 508.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote: 
remote: Create a pull request for 'ft/service-redesign' on GitHub by visiting:
remote:      https://github.com/umbereye27/Bundle-2/pull/new/ft/service-redesign
remote:
To https://github.com/umbereye27/Bundle-2.git
 * [new branch]      ft/service-redesign -> ft/service-redesign

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/service-redesign)    
$ git diff main
diff --git a/service.html b/service.html
new file mode 100644
index 0000000..17ccd55
--- /dev/null
+++ b/service.html
@@ -0,0 +1,12 @@
+<!DOCTYPE html>
+<html lang="en">
+<head>
+    <meta charset="UTF-8">
+    <meta name="viewport" content="width=device-width, initial-scale=1.0">
+    <title>Document</title>        
+</head>
+<body>
+    <h1>Our Service</h1>
+    <h3>We offer web development anset mark: ...skipping...
diff --git a/service.html b/service.html
new file mode 100644
index 0000000..17ccd55
--- /dev/null
+++ b/service.html
@@ -0,0 +1,12 @@
+<!DOCTYPE html>
+<html lang="en">
+<head>
+    <meta charset="UTF-8">
+    <meta name="viewport" content="width=device-width, initial-scale=1.0">
+    <title>Document</title>        
+</head>
+<body>
+    <h1>Our Service</h1>
+    <h3>We offer web development an...skipping...
diff --git a/service.html b/service.html
new file mode 100644
index 0000000..17ccd55
--- /dev/null
+++ b/service.html
@@ -0,0 +1,12 @@
+<!DOCTYPE html>
+<html lang="en">
+<head>
+    <meta charset="UTF-8">
+    <meta name="viewport" content="
width=device-width, initial-scale=1.0">
+    <title>Document</title>        
+</head>
+<body>
+    <h1>Our Service</h1>
+    <h3>We offer web development and mobile app design</h3>
+</body>
+</html>
\ No newline at end of file
set mark: ...skipping...
diff --git a/service.html b/service.html
new file mode 100644
index 0000000..17ccd55
--- /dev/null
+++ b/service.html
@@ -0,0 +1,12 @@
+<!DOCTYPE html>
+<html lang="en">
+<head>
+    <meta charset="UTF-8">
+    <meta name="viewport" content="width=device-width, initial-scale=1.0">
+    <title>Document</title>        
+</head>
+<body>
+    <h1>Our Service</h1>
+    <h3>We offer web development and mobile app design</h3>
+</body>
+</html>
\ No newline at end of file

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/service-redesign)    
$ git merge main
Already up to date.

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/service-redesign)    
$ git status
On branch ft/service-redesign
nothing to commit, working tree clean

Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/service-redesign)
$ git commit -m "Resolved merge conflicts between main and ft/service-redesign"
On branch ft/service-redesign
nothing to commit, working tree clean

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/service-redesign)
$ git push origin ft/service-redesign
Everything up-to-date

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/service-redesign)
$
```

## Bundle 3

### Exercise 1

```bash
Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/service-redesign)
$ git checkout -b ft/team-page
Switched to a new branch 'ft/team-page'

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/team-page)
$ git status
On branch ft/team-page
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        team.html

nothing added to commit but untracked files present (use "git add" to track)

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/team-page)
$ git add .

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/team-page)
$ git commit -m "Add team page"
[ft/team-page 5a213f7] Add team page
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 team.html       

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/team-page)
$ git push
fatal: The current branch ft/team-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/team-page

To have this happen automatically for branches without a tracking       
upstream, see 'push.autoSetupRemote' in 'git help config'.


Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/team-page)
$ git push --set-upstream origin ft/team-page
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done. 
Delta compression using up to 8 threads
Compressing objects: 100% (5/5), done.
Writing objects: 100% (5/5), 688 bytes | 688.00 KiB/s, done.
Total 5 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), done.
remote:
remote: Create a pull request for 'ft/team-page' on GitHub by visiting: 
remote:      https://github.com/umbereye27/Bundle-2/pull/new/ft/team-page
remote:
To https://github.com/umbereye27/Bundle-2.git
 * [new branch]      ft/team-page -> ft/team-page
branch 'ft/team-page' set up to track 'origin/ft/team-page'.

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/team-page)
$ git checkout main
Switched to branch 'main'
Your branch is behind 'origin/main' by 2 commits, and can be fast-forwarded.
  (use "git pull" to update your local branch)

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (main)
$ git checkout -b ft/contact-page
Switched to a new branch 'ft/contact-page'

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/contact-page)        
$ git checkout ft/team-page
Switched to branch 'ft/team-page'
Your branch is up to date with 'origin/ft/team-page'.

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/team-page)
$ git log -1
commit 5a213f753f3a7b6527ef99ace02fc07d327ee682 (HEAD -> ft/team-page, origin/ft/team-page)

    Add team page


    Add team page

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/team-page)
$ git checkout ft/contact-page
Switched to branch 'ft/contact-page'

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/contact-page)
$ git log
commit 9879b06c9af3b9543b5644f79149d2fa804dac32 (HEAD -> ft/contact-page, main)
Author: umbereye27 <carineumbereye7@gmail.com>
Date:   Sun Apr 6 10:55:39 2025 +020

    first commit

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/contact-page)        
$ git cherry-pick 5a213f753f3a7b6527ef99ace02fc07d327ee682
[ft/contact-page 97bb3e2] Add team page
 Date: Sun Apr 6 11:42:26 2025 +0200

 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 team.html       

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/contact-page)        
$ it status
bash: it: command not found

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/contact-page)        
$ git status
On branch ft/contact-page
Untracked files:
  (use "git add <file>..." to include in what will be committed)        
        contact.html

nothing added to commit but untracked files present (use "git add" to track)

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/contact-page)        
$ git add .

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/contact-page)        
$ git commit -m "Add contact page"
[ft/contact-page 3ee99d2] Add contact page
 1 file changed, 11 insertions(+)   
 create mode 100644 contact.html    

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/contact-page)        
$ git push origin ft/contact-page
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done. 
Delta compression using up to 8 threads
Compressing objects: 100% (5/5), done.
Writing objects: 100% (5/5), 631 bytes | 157.00 KiB/s, done.
Total 5 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), done.
remote:
remote: Create a pull request for 'ft/contact-page' on GitHub by visiting:
remote:      https://github.com/umbereye27/Bundle-2/pull/new/ft/contact-page
remote:
To https://github.com/umbereye27/Bundle-2.git
 * [new branch]      ft/contact-page -> ft/contact-page

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/contact-page)        
$ git checkout -b ft/faq-page
Switched to a new branch 'ft/faq-page'

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/faq-page)
$ git status
On branch ft/faq-page
Untracked files:
  (use "git add <file>..." to include in what will be committed)        
        faq.html

nothing added to commit but untracked files present (use "git add" to track)

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/faq-page)
$ git add .

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/faq-page)
$ git commit -m "Add FAQ page"
[ft/faq-page 4ca8a8e] Add FAQ page
 1 file changed, 11 insertions(+)   
 create mode 100644 faq.html        

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/faq-page)
$ git push
fatal: The current branch ft/faq-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/faq-page

To have this happen automatically for branches without a tracking       
upstream, see 'push.autoSetupRemote' in 'git help config'.


Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/faq-page)
$ git push --set-upstream origin ft/faq-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done. 
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 426 bytes | 426.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.    
remote:
remote: Create a pull request for 'ft/faq-page' on GitHub by visiting:  
remote:      https://github.com/umbereye27/Bundle-2/pull/new/ft/faq-pag 
remote:
To https://github.com/umbereye27/Bundle-2.git
 * [new branch]      ft/faq-page -> ft/faq-page
branch 'ft/faq-page' set up to track 'origin/ft/faq-page'.

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/faq-page)
$ git checkout ft/team-page
Switched to branch 'ft/team-page'
Your branch is up to date with 'origin/ft/team-page'.
commit 5a213f753f3a7b6527ef99ace02fc07d327ee682 (HEAD -> ft/team-page, origin/ft/team-page)
Author: umbereye27 <carineumbereye7@gmail.com>
Date:   Sun Apr 6 11:42:26 2025 +0200

    Add team page

Revert "Add team page"e7d1329b264164f74840041c5 (origin/ft/service-redesign, ft/service-redesign)
Author: umbereye27 <carineumbereye7@gmail.com>
Date:   Sun Apr 6 11:16:16 2025 +0200
Revert "Add team page"
    Updated services.h

This reverts commit 5a213f753f3a7b6527ef99ace02fc07d327ee682.
Revert "Add team page"
ional content
#       deleted:    team.html

commit 9879b06c9af3b9543b5644f79149d2fa804dac32 (main)
Author: umbereye27 <carineumbereye7@gmail.com>
Date:   Sun Apr 6 10:55:39 2025 +0200

    first commit
~
~

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/team-page)
$ git revert  5a213f753f3a7b6527ef99ace02fc07d327ee682
hint: Waiting for your editor to close the file...





                     0 [sig] bash 2728! sigpacket::process: Suppressing signal 18 to win32 process (pid 13784)
[ft/team-page 3b91513] Revert "Add team page"
 1 file changed, 0 insertions(+), 0 deletions(-)
 delete mode 100644 team.html

$ git revert  5a213f753f3a7b6527ef99ace02fc07d327ee682
On branch ft/team-page
Your branch is ahead of 'origin/ft/team-page' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/team-page)
$ git commit -m "Revert last team page changes"
On branch ft/team-page
Your branch is ahead of 'origin/ft/team-page' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/team-page)
$ git push origin ft/team-page
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done. 
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 270 bytes | 270.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.    
To https://github.com/umbereye27/Bundle-2.git
   5a213f7..3b91513  ft/team-page -> ft/team-page

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/team-page)
$
```
### Exercise 2
```bash

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (main)
$ git checkout ft/faq-page
Switched to branch 'ft/faq-page'
Your branch is up to date with 'origin/ft/faq-page'.

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/faq-page)
$ 
git checkout -b ft/home-page-redesign
Switched to a new branch 'ft/home-page-redesign'

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/home-page-redesign)  
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:      
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory) 
        modified:   index.html      

no changes added to commit (use "git add" and/or "git commit -a")       

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (main)
$ git add .

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (main)
$ git commit -m "Update home page content"
[main 54e7518] Update home page content
 1 file changed, 1 insertion(+), 1 deletion(-)

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (main)
$ git push origin main
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done. 
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 330 bytes | 330.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
   e1da05a..54e7518  main -> main

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (main)
$ git checkout ft/home-page-redesignSwitched to branch 'ft/home-page-redesign'

   e1da05a..54e7518  main -> main   

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (main)
$ git checkout ft/home-page-redesignSwitched to branch 'ft/home-page-redesign'

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/home-page-redesign)  
$ git rebase main
Successfully rebased and updated refs/heads/ft/home-page-redesign.      

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/home-page-redesign)  
$ git add .

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/home-page-redesign)  
$ git commit -m "Add change on index file"
On branch ft/home-page-redesign
nothing to commit, working tree clean

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/home-page-redesign)  
$ git status
On branch ft/home-page-redesign
Changes not staged for commit:      
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory) 
        modified:   index.html      

no changes added to commit (use "git add" and/or "git commit -a")       

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/home-page-redesign)  
$ git add .

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/home-page-redesign)  
$ git commit -m "Add change on index file"
[ft/home-page-redesign 6054ace] Add change on index file
 1 file changed, 1 insertion(+), 1 deletion(-)

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/home-page-redesign)  
$ git push origin ft/home-page-redesign
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done. 
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 314 bytes | 314.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.   
remote:
remote: Create a pull request for 'ft/home-page-redesign' on GitHub by visiting:
remote:      https://github.com/umbereye27/Bundle-2/pull/new/ft/home-page-redesign
remote:
To https://github.com/umbereye27/Bundle-2.git
 * [new branch]      ft/home-page-redesign -> ft/home-page-redesign     

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/home-page-redesign)  
$
```
## Bundle 4

### Exercise 1
```bash
Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/home-page-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (main)
$ git remote add git-copy https://github.com/umbereye27/Bundle-4.git

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   index.html

no changes added to commit (use "git add" and/or "git commit -a")

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (main)
$ git add .

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)        
        modified:   index.html


Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (main)
$ git commit -m "Update homepage content"
[main 0a4ab75] Update homepage content
 1 file changed, 1 insertion(+), 1 deletion(-)

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (main)
$ git push origin main
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 320 bytes | 160.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/umbereye27/Bundle-2.git
   54e7518..0a4ab75  main -> main

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (main)
$ git push git-copy main
Enumerating objects: 41, done.
Counting objects: 100% (41/41), done.
Delta compression using up to 8 threads
Compressing objects: 100% (39/39), done.
Writing objects: 100% (41/41), 8.09 KiB | 517.00 KiB/s, done.
Total 41 (delta 20), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (20/20), done.
To https://github.com/umbereye27/Bundle-4.git
 * [new branch]      main -> main   

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (main)
$ ^C

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (main)
$
```

### Exerce 2

``` bash
malitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (main)
$ git checkout -b ft/footer
Switched to a new branch 'ft/footer'

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/footer)
$ git status
On branch ft/footer
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        footer.html

nothing added to commit but untracked files present (use "git add" to track)

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/footer)
$ git add .

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/footer)
$ git coomit -m "Add foot file in project"
git: 'coomit' is not a git command. See 'git --help'.

The most similar command is
        commit

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/footer)
$ git commit -m "Add foot file in pr
oject"
[ft/footer b41bb6c] Add foot file in project
 1 file changed, 11 insertions(+)   
 create mode 100644 footer.html     

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/footer)
$ git status
On branch ft/footer
Changes not staged for commit:      
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory) 
        modified:   footer.html     

no changes added to commit (use "git add" and/or "git commit -a")       

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/footer)
$ git add .

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/footer)
$ git commit -m "Add content footer 
file in project"
[ft/footer 784613d] Add content footer file in project
 1 file changed, 3 insertions(+), 1 deletion(-)

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/footer)
$ git push
fatal: The current branch ft/footer has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/footer

To have this happen automatically for branches without a tracking       
upstream, see 'push.autoSetupRemote' in 'git help config'.


Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/footer)
$ git push --set-upstream origin ft/footer
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done. 
Delta compression using up to 8 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 715 bytes | 238.00 KiB/s, done.
Total 6 (delta 3), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (3/3), completed with 1 local object.    
remote:
remote: Create a pull request for 'ft/footer' on GitHub by visiting:    
remote:      https://github.com/umbereye27/Bundle-2/pull/new/ft/footer  
remote:
To https://github.com/umbereye27/Bundle-2.git
 * [new branch]      ft/footer -> ft/footer
branch 'ft/footer' set up to track 'origin/ft/footer'.

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/footer)
$ git push --set-upstream origin ft/footer
branch 'ft/footer' set up to track 'origin/ft/footer'.
Everything up-to-date

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/footer)
$ git status
On branch ft/footer
Your branch is up to date with 'origin/ft/footer'.

nothing to commit, working tree clean

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/footer)
$ git status
On branch ft/footer
Your branch is up to date with 'origin/ft/footer'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory) 
        modified:   footer.html     

no changes added to commit (use "git add" and/or "git commit -a")       

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/footer)
$ git add .

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/footer)
$ git status
On branch ft/footer
Your branch is up to date with 'origin/ft/footer'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   footer.html     


Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/footer)
$ git commit -m "Add content footer file in project"
[ft/footer 28e86cc] Add content footer file in project
 1 file changed, 1 insertion(+), 1 deletion(-)

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/footer)
$ git push --set-upstream origin ft/footer
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done. 
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 333 bytes | 333.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.   
To https://github.com/umbereye27/Bundle-2.git
   784613d..28e86cc  ft/footer -> ft/footer
branch 'ft/footer' set up to track 'origin/ft/footer'.

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/footer)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (main)
$ git checkout -b ft/squashing
Switched to a new branch 'ft/squashing'

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/squashing)
$ git merge --squash ft/footer
Updating 0a4ab75..28e86cc
Fast-forward
Squash commit -- not updating HEAD  
 footer.html | 13 +++++++++++++     
 1 file changed, 13 insertions(+)   
 create mode 100644 footer.html     

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/squashing)
$ git commit -m "footer changes squashing"
[ft/squashing 3d9fd70] footer changes squashing
 1 file changed, 13 insertions(+)   
 create mode 100644 footer.html     

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/squashing)
$ git push origin ft/squashing
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done. 
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 445 bytes | 445.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.    
remote:
remote: Create a pull request for 'ft/squashing' on GitHub by visiting: 
remote:      https://github.com/umbereye27/Bundle-2/pull/new/ft/squashing
remote:
To https://github.com/umbereye27/Bundle-2.git
 * [new branch]      ft/squashing -> ft/squashing

Amalitech@DESKTOP-DPAQHJ3 MINGW64 ~/Desktop/AmaliTech/gitExercisesProject/Bundle-2 (ft/squashing)
```