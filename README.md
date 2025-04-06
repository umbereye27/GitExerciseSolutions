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