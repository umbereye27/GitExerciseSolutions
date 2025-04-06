# Git Exercises

## Bundle One 
### Exercise 1
'''bash
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
'''



### Exercise 2

'''bash
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
'''
