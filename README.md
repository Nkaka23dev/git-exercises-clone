# Gym Git Exercise Solutions 

..This is the GYM exercises for the GYM Rwanda.

## Bundle 1

### exercises 1

...

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises
$ git init
Initialized empty Git repository in C:/Users/TheGym/Desktop/gitExercises/.git/

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (master)
$ git branch -M main

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git status
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        README.md

nothing added to commit but untracked files present (use "git add" to track)

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git add .

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git commit -m "First commit"
[main (root-commit) 2925340] First commit
 1 file changed, 8 insertions(+)
 create mode 100644 README.md

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git remote add origin https://github.com/Nkaka23dev/Gym-Git-Exercise-Solutions.git

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git push -u origin main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 299 bytes | 149.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/Nkaka23dev/Gym-Git-Exercise-Solutions.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git checkout dev 
error: pathspec 'dev' did not match any file(s) known to git

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git checkout -b  dev
Switched to a new branch 'dev'

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git push
fatal: The current branch dev has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin dev

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$  git push --set-upstream origin dev
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote: 
remote: Create a pull request for 'dev' on GitHub by visiting:
remote:      https://github.com/Nkaka23dev/Gym-Git-Exercise-Solutions/pull/new/dev
remote:
To https://github.com/Nkaka23dev/Gym-Git-Exercise-Solutions.git
 * [new branch]      dev -> dev
branch 'dev' set up to track 'origin/dev'.

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git checkout -b test
Switched to a new branch 'test'

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (test)
$ git push
fatal: The current branch test has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin test

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (test)
$  git push --set-upstream origin test
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote: 
remote: Create a pull request for 'test' on GitHub by visiting:
remote:      https://github.com/Nkaka23dev/Gym-Git-Exercise-Solutions/pull/new/test
remote:
To https://github.com/Nkaka23dev/Gym-Git-Exercise-Solutions.git
 * [new branch]      test -> test
branch 'test' set up to track 'origin/test'.

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (test)
$ git push origin --delete test
To https://github.com/Nkaka23dev/Gym-Git-Exercise-Solutions.git
 - [deleted]         test

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (test)
$ git branch
  dev
  main
* test

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (test)
$ git branch -d test
error: Cannot delete branch 'test' checked out at 'C:/Users/TheGym/Desktop/gitExercises'

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (test)
$ git checkout dev
Switched to branch 'dev'
Your branch is up to date with 'origin/dev'.

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git branch -d test
Deleted branch test (was 2925340).

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git branch
* dev
  main

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$

...

#Bundle 1 exercises 2

...
TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git status
On branch dev
Your branch is ahead of 'origin/dev' by 1 commit.
  (use "git push" to publish your local commits)

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        home.html

nothing added to commit but untracked files present (use "git add" to track)

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git add home.html

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git stash
Saved working directory and index state WIP on dev: d748a80 Updaded readMe

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git stash list
stash@{0}: WIP on dev: d748a80 Updaded readMe

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git status
On branch dev
Your branch is ahead of 'origin/dev' by 1 commit.
  (use "git push" to publish your local commits)

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        about.html

nothing added to commit but untracked files present (use "git add" to track)

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git add .

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git stash
Saved working directory and index state WIP on dev: d748a80 Updaded readMe

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git stash list
stash@{0}: WIP on dev: d748a80 Updaded readMe
stash@{1}: WIP on dev: d748a80 Updaded readMe

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git status
On branch dev
Your branch is ahead of 'origin/dev' by 1 commit.
  (use "git push" to publish your local commits)

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        team.html

nothing added to commit but untracked files present (use "git add" to track)

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git add .

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git stash
Saved working directory and index state WIP on dev: d748a80 Updaded readMe

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git stash list
stash@{0}: WIP on dev: d748a80 Updaded readMe
stash@{1}: WIP on dev: d748a80 Updaded readMe
stash@{2}: WIP on dev: d748a80 Updaded readMe

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git stash pop stash@{1}
On branch dev
Your branch is ahead of 'origin/dev' by 1 commit.
  (use "git push" to publish your local commits)

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

Dropped stash@{1} (357dde07ed0c4bb6c189481d0dcbdcd0a3db64e6)

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git stash list
stash@{0}: WIP on dev: d748a80 Updaded readMe
stash@{1}: WIP on dev: d748a80 Updaded readMe

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git stash pop 0
On branch dev
Your branch is ahead of 'origin/dev' by 1 commit.
  (use "git push" to publish your local commits)

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   team.html

Dropped refs/stash@{0} (7829b36eba073f5c8a5083bd4059ce9c046dd85a)

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git stash list
stash@{0}: WIP on dev: d748a80 Updaded readMe

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git status
On branch dev
Your branch is ahead of 'origin/dev' by 1 commit.
  (use "git push" to publish your local commits)

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   team.html


TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git add team.html

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git stash
Saved working directory and index state WIP on dev: d748a80 Updaded readMe

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git stash list
stash@{0}: WIP on dev: d748a80 Updaded readMe
stash@{1}: WIP on dev: d748a80 Updaded readMe

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git add .

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git stash
No local changes to save

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git stash list
stash@{0}: WIP on dev: d748a80 Updaded readMe
stash@{1}: WIP on dev: d748a80 Updaded readMe

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git stash pop 1
On branch dev
Your branch is ahead of 'origin/dev' by 1 commit.
  (use "git push" to publish your local commits)

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   home.html

Dropped refs/stash@{1} (c8943bff9d08ec6397527bc3bbbe1179160ec384)

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git stash pop 0
On branch dev
Your branch is ahead of 'origin/dev' by 1 commit.

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git stash list

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git status
On branch dev
Your branch is ahead of 'origin/dev' by 1 commit.  
  (use "git push" to publish your local commits)   

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   home.html 
        new file:   team.html 

Changes not staged for commit:
  (use "git add/rm <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        deleted:    about.html
        modified:   home.html
        deleted:    team.html


TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git add .

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ gitstatus
bash: gitstatus: command not found

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git status

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git stash
Saved working directory and index state WIP on dev: d748a80 Updaded readMe

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git stash list
stash@{0}: WIP on dev: d748a80 Updaded readMe

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git status
On branch dev
Your branch is ahead of 'origin/dev' by 1 commit.
  (use "git push" to publish your local commits) 

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        About.html

nothing added to commit but untracked files present (use "git add" to track)

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git add .

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git stash
Saved working directory and index state WIP on dev: d748a80 Updaded readMe

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git stash
No local changes to save

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git stash list
stash@{0}: WIP on dev: d748a80 Updaded readMe
stash@{1}: WIP on dev: d748a80 Updaded readMe

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git status
On branch dev
Your branch is ahead of 'origin/dev' by 1 commit.
  (use "git push" to publish your local commits)

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        Team.html

nothing added to commit but untracked files present (use "git add" to track)

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git add .

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git stash
Saved working directory and index state WIP on dev: d748a80 Updaded readMe

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git stash list
stash@{0}: WIP on dev: d748a80 Updaded readMe
stash@{1}: WIP on dev: d748a80 Updaded readMe
stash@{2}: WIP on dev: d748a80 Updaded readMe

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git stash pop stash@{1}
On branch dev
Your branch is ahead of 'origin/dev' by 1 commit.
  (use "git push" to publish your local commits)

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   About.html

Dropped stash@{1} (dd89b145689c5016f468086ac1a6ce0e0699a8ac)

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git stash list
stash@{0}: WIP on dev: d748a80 Updaded readMe
stash@{1}: WIP on dev: d748a80 Updaded readMe

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git stash pop 1
On branch dev
Your branch is ahead of 'origin/dev' by 1 commit.
  (use "git push" to publish your local commits)

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   About.html
        new file:   home.html

Dropped refs/stash@{1} (b8d8895eabbda21d6b5c032c3c81701d1917b746)

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git commit -m "bring back stashed file home and abou"
[dev bcc905a] bring back stashed file home and abou
 2 files changed, 24 insertions(+)
 create mode 100644 About.html
 create mode 100644 home.html

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git push
Enumerating objects: 9, done.
Counting objects: 100% (9/9), done.
Delta compression using up to 4 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (7/7), 1.88 KiB | 384.00 KiB/s, done.
Total 7 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), done.
To https://github.com/Nkaka23dev/Gym-Git-Exercise-Solutions.git
   2925340..bcc905a  dev -> dev

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git stash pop
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   Team.html

Dropped refs/stash@{0} (c3f5dd48f95f9b910d769e23b92961a85c99c54b)

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git reset

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git log
commit bcc905a9a6b64dd285c213afa8ff9b9c0d6e7dce (HEAD -> dev, origin/dev)
Author: Nkaka23dev <nkakaeric96@gmail.com>
Date:   Wed Nov 9 17:44:50 2022 +0200

    bring back stashed file home and abou

commit d748a80f787230d8138d92a3c086eb801e3d3d6d
Author: Nkaka23dev <nkakaeric96@gmail.com>
Date:   Wed Nov 9 17:20:45 2022 +0200

    Updaded readMe

commit 2925340d569dd5dd4ac8a1af22213bf13b1f29e0 (origin/main, main)
Author: Nkaka23dev <nkakaeric96@gmail.com>
Date:   Wed Nov 9 17:15:02 2022 +0200
...skipping...
commit bcc905a9a6b64dd285c213afa8ff9b9c0d6e7dce (HEAD -> dev, origin/dev)
Author: Nkaka23dev <nkakaeric96@gmail.com>
Date:   Wed Nov 9 17:44:50 2022 +0200

    bring back stashed file home and abou

commit d748a80f787230d8138d92a3c086eb801e3d3d6d
Author: Nkaka23dev <nkakaeric96@gmail.com>
Date:   Wed Nov 9 17:20:45 2022 +0200

    Updaded readMe

commit 2925340d569dd5dd4ac8a1af22213bf13b1f29e0 (origin/main, main)
Author: Nkaka23dev <nkakaeric96@gmail.com>
Date:   Wed Nov 9 17:15:02 2022 +0200


TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git log
commit bcc905a9a6b64dd285c213afa8ff9b9c0d6e7dce (HEAD -> dev, origin/dev)
Author: Nkaka23dev <nkakaeric96@gmail.com>
Date:   Wed Nov 9 17:44:50 2022 +0200

    bring back stashed file home and abou

commit d748a80f787230d8138d92a3c086eb801e3d3d6d
Author: Nkaka23dev <nkakaeric96@gmail.com>
Date:   Wed Nov 9 17:20:45 2022 +0200

    Updaded readMe

commit 2925340d569dd5dd4ac8a1af22213bf13b1f29e0 (origin/main, main)
Author: Nkaka23dev <nkakaeric96@gmail.com>
Date:   Wed Nov 9 17:15:02 2022 +0200

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git reset --hard bcc905a9a6b64dd285c213afa8ff9b9c0d6e7dce1~
fatal: ambiguous argument 'bcc905a9a6b64dd285c213afa8ff9b9c0d6e7dce1~': unknown revision or path not in the working tree.
Use '--' to separate paths from revisions, like this:
'git <command> [<revision>...] -- [<file>...]'

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git reset --hard 'bcc905a9a6b64dd285c213afa8ff9b9c0d6e7dce1'
fatal: ambiguous argument 'bcc905a9a6b64dd285c213afa8ff9b9c0d6e7dce1': unknown revision or path not in the working tree.
Use '--' to separate paths from revisions, like this:
'git <command> [<revision>...] -- [<file>...]'

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git reset --hard bcc905a9a6b64dd285c213afa8ff9b9c0d6e7dce1
fatal: ambiguous argument 'bcc905a9a6b64dd285c213afa8ff9b9c0d6e7dce1': unknown revision or path not in the working tree.
Use '--' to separate paths from revisions, like this:
'git <command> [<revision>...] -- [<file>...]'

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git restore d748a80f787230d8138d92a3c086eb801e3d3d6d1~
error: pathspec 'd748a80f787230d8138d92a3c086eb801e3d3d6d1~' did not match any file(s) known to git

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git restore d748a80f787230d8138d92a3c086eb801e3d3d6d1
error: pathspec 'd748a80f787230d8138d92a3c086eb801e3d3d6d1' did not match any file(s) known to 
git

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git reset  d748a80f787230d8138d92a3c086eb801e3d3d6d1
fatal: ambiguous argument 'd748a80f787230d8138d92a3c086eb801e3d3d6d1': unknown revision or path not in the working tree.
Use '--' to separate paths from revisions, like this:
'git <command> [<revision>...] -- [<file>...]'

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git reset --hard
HEAD is now at bcc905a bring back stashed file home and abou

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git add team.html

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git stash 
No local changes to save

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git stash list

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git status
On branch dev
Your branch is up to date with 'origin/dev'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        Team.html

nothing added to commit but untracked files present (use "git add" to track)

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git add .

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git stash
Saved working directory and index state WIP on dev: bcc905a bring back stashed file home and abou

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git stash list
stash@{0}: WIP on dev: bcc905a bring back stashed file home and abou

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git stash pop
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   Team.html

Dropped refs/stash@{0} (dc6af4fd1c44fef4a298d0cddf32857c27f4c86c)

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$ git reset --hard
HEAD is now at bcc905a bring back stashed file home and abou

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (dev)
$
...

### Bundle 2 exercises 2

...
TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/service-redesign)
$ git status
On branch ft/service-redesign
Your branch is up to date with 'origin/ft/service-redesign'.

nothing to commit, working tree clean

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/service-redesign)
$ git log
commit 1435d23fd88fba7cf518b451ad1f3418ae77f02b (HEAD -> ft/service-redesign, origin/ft/service-redesign)
Author: Nkaka23dev <nkakaeric96@gmail.com>

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/service-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   services.html

no changes added to commit (use "git add" and/or "git commit -a")

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git add .

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git commit -m "changed service"
[main bdb1587] changed service
 1 file changed, 1 insertion(+)

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 338 bytes | 338.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/Nkaka23dev/Gym-Git-Exercise-Solutions.git
   246e142..bdb1587  main -> main

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git branch

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git branch
  dev
  ft/bundle-2
  ft/service-redesign
* main

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git push origin --delete ft/service-redesign
To https://github.com/Nkaka23dev/Gym-Git-Exercise-Solutions.git
 - [deleted]         ft/service-redesign

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git branch -d ft/service-redesign
error: The branch 'ft/service-redesign' is not fully merged.

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git checkout main
Already on 'main'
Your branch is up to date with 'origin/main'.

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git pull
remote: Enumerating objects: 4, done.
remote: Counting objects: 100% (4/4), done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 2 (delta 1), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (2/2), 704 bytes | 64.00 KiB/s, done.
From https://github.com/Nkaka23dev/Gym-Git-Exercise-Solutions
   bdb1587..aabf40e  main       -> origin/main
Updating bdb1587..aabf40e
Fast-forward
 README.md | 2 +-
 1 file changed, 1 insertion(+), 1 deletion(-)

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git checkout -b ft/service-redesign
Switched to a new branch 'ft/service-redesign'

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/service-redesign)
$ git status
On branch ft/service-redesign
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   services.html

no changes added to commit (use "git add" and/or "git commit -a")

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/service-redesign)
$ git add --all

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/service-redesign)
$ git commit -m "modified services"
[ft/service-redesign dada12f] modified services
 1 file changed, 5 insertions(+)

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/service-redesign)
$ git push
fatal: The current branch ft/service-redesign has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/service-redesign

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/service-redesign)
$ git push --set-upstream origin ft/service-redesign
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 325 bytes | 81.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
remote:
remote: Create a pull request for 'ft/service-redesign' on GitHub by visiting:
remote:      https://github.com/Nkaka23dev/Gym-Git-Exercise-Solutions/pull/new/ft/service-redesign
remote:
To https://github.com/Nkaka23dev/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/service-redesign -> ft/service-redesign
branch 'ft/service-redesign' set up to track 'origin/ft/service-redesign'.

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/service-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   services.html

no changes added to commit (use "git add" and/or "git commit -a")

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git add --all

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git commit -m services on main"
> ^C

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git commit -m 'services on main"
> ^C

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git sttaus
git: 'sttaus' is not a git command. See 'git --help'.

The most similar command is
        status

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   services.html


TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git commit -m "changed services form main"
[main b279826] changed services form main
 1 file changed, 1 insertion(+)

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git branch
  dev
  ft/bundle-2
  ft/service-redesign
* main

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git checkout ft/service-redesign
Switched to branch 'ft/service-redesign'
Your branch is up to date with 'origin/ft/service-redesign'.

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/service-redesign)
$ git merge main
Auto-merging services.html
CONFLICT (content): Merge conflict in services.html
Automatic merge failed; fix conflicts and then commit the result.
TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/service-redesign|MERGING)
$ git add .

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/service-redesign|MERGING)
$ git commit -m "updated"
[ft/service-redesign f13ae85] updated

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/service-redesign)
$
... 


## Bundle 3

### exercises 1

...
TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/service-redesign|MERGING)
$ git status
On branch ft/service-redesign
Your branch is up to date with 'origin/ft/service-redesign'.

All conflicts fixed but you are still merging.
  (use "git commit" to conclude merge)

Changes to be committed:
        modified:   services.html


TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/service-redesign)
$ git checkout -b ft/team-page
Switched to a new branch 'ft/team-page'

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/team-page)
$ git branch
  dev
  ft/bundle-2
  ft/service-redesign
* ft/team-page
  main

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/team-page)
$ git status
On branch ft/team-page
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        team.html

no changes added to commit (use "git add" and/or "git commit -a")

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/team-page)
$ git add .

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/team-page)
$ git commit -m "added team pages and modified it"
[ft/team-page 4f06e01] added team pages and modified it
 2 files changed, 31 insertions(+)
 create mode 100644 team.html

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/team-page)
$ git push
fatal: The current branch ft/team-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/team-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/team-page)
$  git push --set-upstream origin ft/team-page
Enumerating objects: 17, done.
Counting objects: 100% (16/16), done.
Delta compression using up to 4 threads
Compressing objects: 100% (11/11), done.
Writing objects: 100% (11/11), 2.54 KiB | 520.00 KiB/s, done.
Total 11 (delta 6), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (6/6), completed with 3 local objects.
remote: 
remote: Create a pull request for 'ft/team-page' on GitHub by visiting:
remote:      https://github.com/Nkaka23dev/Gym-Git-Exercise-Solutions/pull/new/ft/team-page    
remote:
To https://github.com/Nkaka23dev/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/team-page -> ft/team-page
branch 'ft/team-page' set up to track 'origin/ft/team-page'.

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/team-page)
$

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/team-page)
$

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/team-page)
$ git checkout main
Switched to branch 'main'
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git checkout -b ft/contact-page
Switched to a new branch 'ft/contact-page'

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/contact-page)
$ git checkout ft/team-page
Switched to branch 'ft/team-page'
Your branch is up to date with 'origin/ft/team-page'.

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/team-page)
$ git log
commit 4f06e011fe4587f54d5c34c19b30fe23b43e7957 (HEAD -> ft/team-page, origin/ft/team-page)
Author: Nkaka23dev <nkakaeric96@gmail.com>
Date:   Thu Nov 10 12:36:13 2022 +0200

    added team pages and modified it

commit f13ae8541bb06a23cc2e444883cba240ae3b525f (ft/service-redesign)
Merge: dada12f b279826
Author: Nkaka23dev <nkakaeric96@gmail.com>
Date:   Thu Nov 10 12:27:40 2022 +0200

    updated

commit b27982637e0074dc1786c86343810e7417beb17f (main, ft/contact-page)
Author: Nkaka23dev <nkakaeric96@gmail.com>

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/team-page)
$ git checkout ft/contact-page
Switched to branch 'ft/contact-page'

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/contact-page)
$ git cherry-pick 4f06e011fe4587f54d5c34c19b30fe23b43e79571
fatal: bad revision '4f06e011fe4587f54d5c34c19b30fe23b43e79571'

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/contact-page)
$ git cherry-pick '4f06e011fe4587f54d5c34c19b30fe23b43e79571'~
fatal: bad revision '4f06e011fe4587f54d5c34c19b30fe23b43e79571~'

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/contact-page)
$ git cherry-pick 4f06e011fe4587f54d5c34c19b30fe23b43e79571
fatal: bad revision '4f06e011fe4587f54d5c34c19b30fe23b43e79571'

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/contact-page)
$ git log
commit b27982637e0074dc1786c86343810e7417beb17f (HEAD -> ft/contact-page, main)
Author: Nkaka23dev <nkakaeric96@gmail.com>
Date:   Thu Nov 10 12:07:24 2022 +0200

    changed services form main

commit aabf40ed7320ca429ea03675e0ebaf2a35ec0366 (origin/main)
Merge: bdb1587 2e98b2e
Author: ericnkaka <62412678+Nkaka23dev@users.noreply.github.com>
Date:   Thu Nov 10 11:58:10 2022 +0200

    Merge pull request #1 from Nkaka23dev/dev

    Bundle 1 exercises


TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/contact-page)
$

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/contact-page)
$ git branch
  dev
  ft/bundle-2
* ft/contact-page
  ft/service-redesign
  ft/team-page
  main

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/contact-page)
$ git checkout ft/team-page
Switched to branch 'ft/team-page'
Your branch is up to date with 'origin/ft/team-page'.

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/team-page)
$ git log
commit 4f06e011fe4587f54d5c34c19b30fe23b43e7957 (HEAD -> ft/team-page, origin/ft/team-page)
Author: Nkaka23dev <nkakaeric96@gmail.com>
Date:   Thu Nov 10 12:36:13 2022 +0200

    added team pages and modified it

commit f13ae8541bb06a23cc2e444883cba240ae3b525f (ft/service-redesign)
Merge: dada12f b279826
Author: Nkaka23dev <nkakaeric96@gmail.com>
Date:   Thu Nov 10 12:27:40 2022 +0200

    updated

commit b27982637e0074dc1786c86343810e7417beb17f (main, ft/contact-page)
Author: Nkaka23dev <nkakaeric96@gmail.com>

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/team-page)
$

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/team-page)
$ git checkout ft/contact-page
Switched to branch 'ft/contact-page'

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/contact-page)
$ git cherry-pick 4f06e011fe4587f54d5c34c19b30fe23b43e79571~
fatal: bad revision '4f06e011fe4587f54d5c34c19b30fe23b43e79571~'

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/contact-page)
$ git cherry-pick 4f06e011fe4587f54d5c34c19b30fe23b43e79571
fatal: bad revision '4f06e011fe4587f54d5c34c19b30fe23b43e79571'

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/contact-page)
$ git checkout ft/team-page
Switched to branch 'ft/team-page'
Your branch is up to date with 'origin/ft/team-page'.

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/team-page)
$ git log
commit 4f06e011fe4587f54d5c34c19b30fe23b43e7957 (HEAD -> ft/team-page, origin/ft/team-page)
Author: Nkaka23dev <nkakaeric96@gmail.com>
Date:   Thu Nov 10 12:36:13 2022 +0200

    added team pages and modified it

commit f13ae8541bb06a23cc2e444883cba240ae3b525f (ft/service-redesign)
Merge: dada12f b279826
Author: Nkaka23dev <nkakaeric96@gmail.com>
Date:   Thu Nov 10 12:27:40 2022 +0200

    updated

commit b27982637e0074dc1786c86343810e7417beb17f (main, ft/contact-page)
Author: Nkaka23dev <nkakaeric96@gmail.com>

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/team-page)
$ git cherry-pick commit 4f06e011fe4587f54d5c34c19b30fe23b43e7957
fatal: bad revision 'commit'

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/team-page)
$ git cherry-pick 4f06e011fe4587f54d5c34c19b30fe23b43e7957
The previous cherry-pick is now empty, possibly due to conflict resolution.
If you wish to commit it anyway, use:

    git commit --allow-empty

Otherwise, please use 'git cherry-pick --skip'
On branch ft/team-page
Your branch is up to date with 'origin/ft/team-page'.

You are currently cherry-picking commit 4f06e01.
  (all conflicts fixed: run "git cherry-pick --continue")
  (use "git cherry-pick --skip" to skip this patch)
  (use "git cherry-pick --abort" to cancel the cherry-pick operation)

nothing to commit, working tree clean

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/team-page|CHERRY-PICKING)
$ git checkout ft/contact-page
Switched to branch 'ft/contact-page'
warning: cancelling a cherry picking in progress

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/contact-page)
$ git cherry-pick 4f06e011fe4587f54d5c34c19b30fe23b43e7957
Auto-merging README.md

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/contact-page|CHERRY-PICKING)
$ git status
On branch ft/contact-page
You are currently cherry-picking commit 4f06e01.
  (fix conflicts and run "git cherry-pick --continue")
  (use "git cherry-pick --skip" to skip this patch)
  (use "git cherry-pick --abort" to cancel the cherry-pick operation)

Changes to be committed:
        new file:   team.html

Unmerged paths:
  (use "git add <file>..." to mark resolution)
        both modified:   README.md


TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/contact-page|CHERRY-PICKING)
$ git checkout ft/team-page
error: you need to resolve your current index first
README.md: needs merge

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/contact-page|CHERRY-PICKING)
$ git cherry-pick 4f06e011fe4587f54d5c34c19b30fe23b43e7957
error: Cherry-picking is not possible because you have unmerged files.
hint: Fix them up in the work tree, and then use 'git add/rm <file>'
hint: as appropriate to mark resolution and make a commit.
fatal: cherry-pick failed

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/contact-page|CHERRY-PICKING)
$ git status
On branch ft/contact-page
You are currently cherry-picking commit 4f06e01.
  (fix conflicts and run "git cherry-pick --continue")
  (use "git cherry-pick --skip" to skip this patch)
  (use "git cherry-pick --abort" to cancel the cherry-pick operation)

Changes to be committed:
        new file:   team.html

Unmerged paths:
  (use "git add <file>..." to mark resolution)
        both modified:   README.md


TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/contact-page|CHERRY-PICKING)
$ git cherry-pick --skip

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/contact-page)
$ git cherry-pick --abort
error: no cherry-pick or revert in progress
fatal: cherry-pick failed

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/contact-page)
$ git checkout ft/team-page
Switched to branch 'ft/team-page'
Your branch is up to date with 'origin/ft/team-page'.

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/team-page)
$ git checkout ft/contact-page
Switched to branch 'ft/contact-page'

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/contact-page)
$ git status
On branch ft/contact-page
nothing to commit, working tree clean

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/contact-page)
$ git checkout ft/team-page
Switched to branch 'ft/team-page'
Your branch is up to date with 'origin/ft/team-page'.

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/team-page)
$ git status
On branch ft/team-page
Your branch is up to date with 'origin/ft/team-page'.

nothing to commit, working tree clean

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/team-page)
$ git branch
  dev
  ft/bundle-2
  ft/contact-page
  ft/service-redesign
* ft/team-page
  main

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/team-page)
$ git status
On branch ft/team-page
Your branch is up to date with 'origin/ft/team-page'.

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/team-page)
$ git checkout ft/team-page 
Already on 'ft/team-page'
Your branch is up to date with 'origin/ft/team-page'.

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/team-page)
$ git log
commit 4f06e011fe4587f54d5c34c19b30fe23b43e7957 (HEAD -> ft/team-page, origin/ft/team-page)
Author: Nkaka23dev <nkakaeric96@gmail.com>
Date:   Thu Nov 10 12:36:13 2022 +0200

    added team pages and modified it

commit f13ae8541bb06a23cc2e444883cba240ae3b525f (ft/service-redesign)
Merge: dada12f b279826
Author: Nkaka23dev <nkakaeric96@gmail.com>
Date:   Thu Nov 10 12:27:40 2022 +0200

    updated

commit b27982637e0074dc1786c86343810e7417beb17f (main, ft/contact-page)
Author: Nkaka23dev <nkakaeric96@gmail.com>

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/team-page)
$

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/team-page)
$ git checkout -b ft/contact-page
fatal: a branch named 'ft/contact-page' already exists

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/team-page)
$ git checkout ft/contact-page
Switched to branch 'ft/contact-page'

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/contact-page)
$ git cherry-check  4f06e011fe4587f54d5c34c19b30fe23b43e7957
git: 'cherry-check' is not a git command. See 'git --help'.

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/contact-page)
$ git cherry-pick  4f06e011fe4587f54d5c34c19b30fe23b43e7957
Auto-merging README.md
CONFLICT (content): Merge conflict in README.md
error: could not apply 4f06e01... added team pages and modified it
hint: After resolving the conflicts, mark them with
hint: "git add/rm <pathspec>", then run
hint: "git cherry-pick --continue".
hint: You can instead skip this commit with "git cherry-pick --skip".
hint: To abort and get back to the state before "git cherry-pick",
hint: run "git cherry-pick --abort".

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/contact-page|CHERRY-PICKING)
$ git cherry-pick  4f06e011fe4587f54d5c34c19b30fe23b43e7957
error: your local changes would be overwritten by cherry-pick.
hint: commit your changes or stash them to proceed.
fatal: cherry-pick failed

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/contact-page|CHERRY-PICKING)
$ git status
On branch ft/contact-page
You are currently cherry-picking commit 4f06e01.
  (all conflicts fixed: run "git cherry-pick --continue")
  (use "git cherry-pick --skip" to skip this patch)
  (use "git cherry-pick --abort" to cancel the cherry-pick operation)

Changes to be committed:
        modified:   README.md
        new file:   team.html


TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/contact-page|CHERRY-PICKING)
$ git checkout main
Switched to branch 'main'
warning: cancelling a cherry picking in progress
M       README.md
A       team.html
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git add .

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git commit -m "upfdated readMe"
[main c013188] upfdated readMe
 2 files changed, 224 insertions(+)
 create mode 100644 team.html

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git push
To https://github.com/Nkaka23dev/Gym-Git-Exercise-Solutions.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/Nkaka23dev/Gym-Git-Exercise-Solutions.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git pull
remote: Enumerating objects: 2, done.
remote: Counting objects: 100% (2/2), done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 2 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (2/2), 1.23 KiB | 179.00 KiB/s, done.
From https://github.com/Nkaka23dev/Gym-Git-Exercise-Solutions
   aabf40e..0c4bfe9  main       -> origin/main
Auto-merging README.md
CONFLICT (content): Merge conflict in README.md
Automatic merge failed; fix conflicts and then commit the result.

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main|MERGING)
$ git add .

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main|MERGING)
$ git commit -m ""
Aborting commit due to empty commit message.

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main|MERGING)
$ git commit -m "adde content on readMe"
[main 6f54f35] adde content on readMe

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git push
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 519 bytes | 259.00 KiB/s, done.
Total 4 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/Nkaka23dev/Gym-Git-Exercise-Solutions.git
   0c4bfe9..6f54f35  main -> main

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git checkout ft/team-page
Switched to branch 'ft/team-page'
Your branch is up to date with 'origin/ft/team-page'.

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/team-page)
$ git log
commit 4f06e011fe4587f54d5c34c19b30fe23b43e7957 (HEAD -> ft/team-page, origin/ft/team-page)
Author: Nkaka23dev <nkakaeric96@gmail.com>
Date:   Thu Nov 10 12:36:13 2022 +0200

    added team pages and modified it

commit f13ae8541bb06a23cc2e444883cba240ae3b525f (ft/service-redesign)
Merge: dada12f b279826
Author: Nkaka23dev <nkakaeric96@gmail.com>
Date:   Thu Nov 10 12:27:40 2022 +0200

    updated

commit b27982637e0074dc1786c86343810e7417beb17f (ft/contact-page)
Author: Nkaka23dev <nkakaeric96@gmail.com>

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/team-page)
$

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/team-page)
$ git checkout ft/contact-page
Switched to branch 'ft/contact-page'

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/contact-page)
$ git cherry-pick commit 4f06e011fe4587f54d5c34c19b30fe23b43e7957
fatal: bad revision 'commit'

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/contact-page)
$ git cherry-pick 4f06e011fe4587f54d5c34c19b30fe23b43e7957
Auto-merging README.md
CONFLICT (content): Merge conflict in README.md
error: could not apply 4f06e01... added team pages and modified it
hint: After resolving the conflicts, mark them with
hint: "git add/rm <pathspec>", then run
hint: "git cherry-pick --continue".
hint: You can instead skip this commit with "git cherry-pick --skip".
hint: To abort and get back to the state before "git cherry-pick",
hint: run "git cherry-pick --abort".

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/contact-page|CHERRY-PICKING)
$ git cherry-pick --skip

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/contact-page)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

...
## Bundle 3

### exercises 2

...
heGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main|MERGING)
$ git add .

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main|MERGING)
$ git commit -m ""
Aborting commit due to empty commit message.

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main|MERGING)
$ git commit -m "adde content on readMe"
[main 6f54f35] adde content on readMe

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git push
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 519 bytes | 259.00 KiB/s, done.
Total 4 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/Nkaka23dev/Gym-Git-Exercise-Solutions.git
   0c4bfe9..6f54f35  main -> main

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git checkout ft/team-page
Switched to branch 'ft/team-page'
Your branch is up to date with 'origin/ft/team-page'.

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/team-page)
$ git log
commit 4f06e011fe4587f54d5c34c19b30fe23b43e7957 (HEAD -> ft/team-page, origin/ft/team-page)
Author: Nkaka23dev <nkakaeric96@gmail.com>
Date:   Thu Nov 10 12:36:13 2022 +0200

    added team pages and modified it

commit f13ae8541bb06a23cc2e444883cba240ae3b525f (ft/service-redesign)
Merge: dada12f b279826
Author: Nkaka23dev <nkakaeric96@gmail.com>
Date:   Thu Nov 10 12:27:40 2022 +0200

    updated

commit b27982637e0074dc1786c86343810e7417beb17f (ft/contact-page)
Author: Nkaka23dev <nkakaeric96@gmail.com>

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/team-page)
$

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/team-page)
$ git checkout ft/contact-page
Switched to branch 'ft/contact-page'

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/contact-page)
$ git cherry-pick commit 4f06e011fe4587f54d5c34c19b30fe23b43e7957
fatal: bad revision 'commit'

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/contact-page)
$ git cherry-pick 4f06e011fe4587f54d5c34c19b30fe23b43e7957
Auto-merging README.md
CONFLICT (content): Merge conflict in README.md
error: could not apply 4f06e01... added team pages and modified it
hint: After resolving the conflicts, mark them with
hint: "git add/rm <pathspec>", then run

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git add .

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git commit -m "updated ReadMe"
[main 318e42f] updated ReadMe
 1 file changed, 531 insertions(+)

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git branch
  dev
  ft/bundle-2

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/contact-page)
$ git status
On branch ft/contact-page
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        contact.html

nothing added to commit but untracked files present (use "git add" to track)

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/contact-page)
$ git add .

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/contact-page)
$ git commit -m "added contact page"
[ft/contact-page d32fff2] added contact page
 1 file changed, 12 insertions(+)
 create mode 100644 contact.html

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/contact-page)
$ git push
fatal: The current branch ft/contact-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/contact-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/contact-page)
$   git push --set-upstream origin ft/contact-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 469 bytes | 469.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/contact-page' on GitHub by visiting:
remote:      https://github.com/Nkaka23dev/Gym-Git-Exercise-Solutions/pull/new/ft/contact-page 

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/faq-page)
$ git add .

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/faq-page)
$ git commit -m "created faq pages"
[ft/faq-page 8473371] created faq pages
 1 file changed, 12 insertions(+)      
 create mode 100644 faq.html

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/faq-page)
$ git checkout ft/team-page
Switched to branch 'ft/team-page'
Your branch is up to date with 'origin/ft/team-page'.

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/team-page)
$ git log
commit 4f06e011fe4587f54d5c34c19b30fe23b43e7957 (HEAD -> ft/team-page, origin/ft/team-page)
Author: Nkaka23dev <nkakaeric96@gmail.com>
Date:   Thu Nov 10 12:36:13 2022 +0200

    added team pages and modified it

commit f13ae8541bb06a23cc2e444883cba240ae3b525f (ft/service-redesign)
Merge: dada12f b279826
Author: Nkaka23dev <nkakaeric96@gmail.com>
Date:   Thu Nov 10 12:27:40 2022 +0200

    updated

commit b27982637e0074dc1786c86343810e7417beb17f
Author: Nkaka23dev <nkakaeric96@gmail.com>

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/team-page)
$

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/team-page)
$ git checkout ft/faq-page
Switched to branch 'ft/faq-page'

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/faq-page)
$ git revert 4f06e011fe4587f54d5c34c19b30fe23b43e7957
Auto-merging README.md
CONFLICT (content): Merge conflict in README.md
error: could not revert 4f06e01... added team pages and modified it
hint: After resolving the conflicts, mark them with
hint: "git add/rm <pathspec>", then run
hint: "git revert --continue".
hint: You can instead skip this commit with "git revert --skip".
hint: To abort and get back to the state before "git revert",
hint: run "git revert --abort".

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/faq-page|REVERTING)
$ git revert 4f06e011fe4587f54d5c34c19b30fe23b43e7957
error: your local changes would be overwritten by revert.
hint: commit your changes or stash them to proceed.
fatal: revert failed

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/faq-page|REVERTING)
$ git stash
Saved working directory and index state WIP on ft/faq-page: 8473371 created faq pages

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/faq-page)
$ git stash npop
fatal: unknown subcommand: npop

usage: git stash list [<options>]
   or: git stash show [<options>] [<stash>]
   or: git stash drop [-q|--quiet] [<stash>]
   or: git stash ( pop | apply ) [--index] [-q|--quiet] [<stash>]
   or: git stash branch <branchname> [<stash>]
   or: git stash clear
   or: git stash [push [-p|--patch] [-S|--staged] [-k|--[no-]keep-index] [-q|--quiet]
                 [-u|--include-untracked] [-a|--all] [-m|--message <message>]
                 [--pathspec-from-file=<file> [--pathspec-file-nul]]
                 [--] [<pathspec>...]]
   or: git stash save [-p|--patch] [-S|--staged] [-k|--[no-]keep-index] [-q|--quiet]
                 [-u|--include-untracked] [-a|--all] [<message>]


TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/faq-page)
$ git stash pop
On branch ft/faq-page
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")
Dropped refs/stash@{0} (cf75e31075e7f7304ad728512c0dc4a756e66f0e)

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/faq-page)
$ git stash pop
No stash entries found.

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/faq-page)
$ git stash pop
No stash entries found.

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/faq-page)
$ git stash pop
No stash entries found.

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/faq-page)
$ git revert commit 4f06e011fe4587f54d5c34c19b30fe23b43e7957
fatal: bad revision 'commit'

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/faq-page)
$ git revert  4f06e011fe4587f54d5c34c19b30fe23b43e7957
error: Your local changes to the following files would be overwritten by merge:
        README.md
Please commit your changes or stash them before you merge.
Aborting
fatal: revert failed

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/faq-page)
$ git commit -m "all changes"
On branch ft/faq-page
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)


E325: ATTENTION
Found a swap file by the name "~/Desktop/gitExercises/.git/.COMMIT_EDITMSG.swp"
          owned by: TheGym   dated: Thu Nov 10 12:25:12 2022
         file name: ~TheGym/Desktop/gitExercises/.git/COMMIT_EDITMSG
          modified: YES
         user name: TheGym   host name: DESKTOP-0FJL824
        process ID: 964
While opening file "/c/Users/TheGym/Desktop/gitExercises/.git/COMMIT_EDITMSG"
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/faq-page)
$ git add .

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/faq-page)
$ git commit -m "all changes"
[ft/faq-page 8166db2] all changes
 1 file changed, 227 insertions(+)

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/faq-page)
$ git revert  4f06e011fe4587f54d5c34c19b30fe23b43e7957
hint: Waiting for your editor to close the file... Vim: Error reading input, exiting...        
Vim: Finished.

error: There was a problem with the editor 'vi'.
Please supply the message using either -m or -F option.

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/faq-page)
$ git commit -m "all changes"
[ft/faq-page 92751a0] all changes
 1 file changed, 17 deletions(-)

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/faq-page)
$ git revert  4f06e011fe4587f54d5c34c19b30fe23b43e7957
On branch ft/faq-page
nothing to commit, working tree clean

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/faq-page)
$ git push
fatal: The current branch ft/faq-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/faq-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/faq-page)
$  git push --set-upstream origin ft/faq-page~
fatal: invalid refspec 'ft/faq-page~'

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/faq-page)
$  git push --set-upstream origin ft/faq-page
Enumerating objects: 11, done.
Counting objects: 100% (11/11), done.
Delta compression using up to 4 threads
Compressing objects: 100% (9/9), done.
Writing objects: 100% (9/9), 2.12 KiB | 1.06 MiB/s, done.
Total 9 (delta 5), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (5/5), completed with 2 local objects.
remote:
remote: Create a pull request for 'ft/faq-page' on GitHub by visiting:
remote:      https://github.com/Nkaka23dev/Gym-Git-Exercise-Solutions/pull/new/ft/faq-page     
remote:
To https://github.com/Nkaka23dev/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/faq-page -> ft/faq-page
branch 'ft/faq-page' set up to track 'origin/ft/faq-page'.

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/faq-page)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
...

## Bundle 3

### exercises 2

...
TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign|REBASE 3/4)       
$ git status
On branch ft/bundle-2
Your branch is up to date with 'origin/ft/bundle-2'.

Last commands done (3 commands done):
   pick 8473371 created faq pages
   pick 8166db2 all changes
  (see more in file .git/rebase-merge/done)
Next command to do (1 remaining command):
   pick 92751a0 all changes
  (use "git rebase --edit-todo" to view and edit)
You are currently editing a commit while rebasing branch 'ft/home-page-redesign' on 'd06de9f'.
  (use "git commit --amend" to amend the current commit)
  (use "git rebase --continue" once you are satisfied with your changes)

nothing to commit, working tree clean

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign|REBASE 3/4)       
$ git rebase main
fatal: It seems that there is already a rebase-merge directory, and
I wonder if you are in the middle of another rebase.  If that is the
case, please try
        git rebase (--continue | --abort | --skip)
If that is not the case, please
        rm -fr ".git/rebase-merge"
and run me again.  I am stopping in case you still have something
valuable there.


TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign|REBASE 3/4)       
$ git rebase --skip
Auto-merging README.md
CONFLICT (content): Merge conflict in README.md
error: could not apply 92751a0... all changes
hint: Resolve all conflicts manually, mark them as resolved with
hint: "git add/rm <conflicted_files>", then run "git rebase --continue".
hint: You can instead skip this commit: run "git rebase --skip".
hint: To abort and get back to the state before "git rebase", run "git rebase --abort".        
Could not apply 92751a0... all changes

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign|REBASE 4/4)       
$ git add .

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign|REBASE 4/4)       
$ git commit -m "rebasing"
[ft/bundle-2 e96c2ab] rebasing
 1 file changed, 84 insertions(+), 1 deletion(-)

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign|REBASE 4/4)       
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 834 bytes | 417.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/Nkaka23dev/Gym-Git-Exercise-Solutions.git
   f474bd8..e96c2ab  ft/bundle-2 -> ft/bundle-2

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign|REBASE 4/4)       
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign|REBASE 4/4)       
$ git branch
  dev
  ft/bundle-2
  ft/contact-page
  ft/faq-page
  ft/home-page-redesign
  ft/service-redesign
  ft/team-page
* main

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign|REBASE 4/4)
$ git push origin --delete  ft/home-page-redesign
error: unable to delete 'ft/home-page-redesign': remote ref does not exist
error: failed to push some refs to 'https://github.com/Nkaka23dev/Gym-Git-Exercise-Solutions.git'

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign|REBASE 4/4)       
$ git branch -D  ft/home-page-redesign
Deleted branch ft/home-page-redesign (was 92751a0).

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign|REBASE 4/4)       
$ git branch
  dev
  ft/bundle-2
  ft/contact-page
  ft/faq-page
  ft/service-redesign
  ft/team-page
* main

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign|REBASE 4/4)       
$ git checkout main
Already on 'main'
Your branch is up to date with 'origin/main'.

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign|REBASE 4/4)       
$ git rebase
fatal: It seems that there is already a rebase-merge directory, and
I wonder if you are in the middle of another rebase.  If that is the

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git checkout ft/faq-page
Switched to branch 'ft/faq-page'
Your branch is up to date with 'origin/ft/faq-page'.

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/faq-page)
$ git checkout -b ft/home-page-redesign
fatal: a branch named 'ft/home-page-redesign' already exists

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/faq-page)
$ git push origin --delete ft/home-page-redesign
error: unable to delete 'ft/home-page-redesign': remote ref does not exist
error: failed to push some refs to 'https://github.com/Nkaka23dev/Gym-Git-Exercise-Solutions.git'

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/faq-page)
$ git checkout -b  ft/home-page-redesign
fatal: a branch named 'ft/home-page-redesign' already exists

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/faq-page)


TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/faq-page)
$ git branch -D ft/home-page-redesign
Deleted branch ft/home-page-redesign (was 92751a0).

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/faq-page)
$ git checkout -b  ft/home-page-redesign
Switched to a new branch 'ft/home-page-redesign'

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign)
$ git push
fatal: The current branch ft/home-page-redesign has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/home-page-redesign

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign)
$   git push --set-upstream origin ft/home-page-redesign
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'ft/home-page-redesign' on GitHub by visiting:
remote:      https://github.com/Nkaka23dev/Gym-Git-Exercise-Solutions/pull/new/ft/home-page-redesign
remote:
To https://github.com/Nkaka23dev/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/home-page-redesign -> ft/home-page-redesign
branch 'ft/home-page-redesign' set up to track 'origin/ft/home-page-redesign'.

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   home.html

no changes added to commit (use "git add" and/or "git commit -a")

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git add .

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git checkout"
> ^C

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git checkout
M       home.html
Your branch is up to date with 'origin/main'.

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git checkout ft/home-page-redesign
error: Your local changes to the following files would be overwritten by checkout:
        home.html
Please commit your changes or stash them before you switch branches.
Aborting

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git commit -m "change some content on the main page"
[main 02fd0e1] change some content on the main page
 1 file changed, 1 insertion(+), 1 deletion(-)

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git checkout ft/home-page-redesign
Switched to branch 'ft/home-page-redesign'
Your branch is up to date with 'origin/ft/home-page-redesign'.

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign)
$ git log
commit 92751a0fb7dfb0724ac3e5ad53f11a45e2b380e3 (HEAD -> ft/home-page-redesign, origin/ft/home-page-redesign, origin/ft/faq-page, ft/faq-page)
Author: Nkaka23dev <nkakaeric96@gmail.com>
Date:   Thu Nov 10 14:24:36 2022 +0200

    all changes

commit 8166db2af6bd9bd996566551c7820481fb6dc1f6
Author: Nkaka23dev <nkakaeric96@gmail.com>
Date:   Thu Nov 10 14:23:42 2022 +0200

    all changes

commit 84733712ad2aefd63f2f5951200e1acacd2f9cb1
Author: Nkaka23dev <nkakaeric96@gmail.com>
Date:   Thu Nov 10 14:18:18 2022 +0200

    created faq pages

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign)
$ git rebase maqin
fatal: invalid upstream 'maqin'

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign)
$ git rebase main
Auto-merging README.md
CONFLICT (content): Merge conflict in README.md
error: could not apply 8166db2... all changes
hint: Resolve all conflicts manually, mark them as resolved with
hint: "git add/rm <conflicted_files>", then run "git rebase --continue".



E325: ATTENTION
Found a swap file by the name "~/Desktop/gitExercises/.git/.COMMIT_EDITMSG.swp"
          owned by: TheGym   dated: Thu Nov 10 12:25:12 2022
         file name: ~TheGym/Desktop/gitExercises/.git/COMMIT_EDITMSG
          modified: YES
         user name: TheGym   host name: DESKTOP-0FJL824
hint: You can instead skip this commit: run "git rebase --skip".
hint: To abort and get back to the state before "git rebase", run "git rebase --abort".        
Could not apply 8166db2... all changes

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign|REBASE 3/4)       
$ git rebase main
fatal: It seems that there is already a rebase-merge directory, and
I wonder if you are in the middle of another rebase.  If that is the
case, please try
        git rebase (--continue | --abort | --skip)
If that is not the case, please
        rm -fr ".git/rebase-merge"
and run me again.  I am stopping in case you still have something
valuable there.


TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign|REBASE 3/4)       
$ git rebase --continue
hint: Waiting for your editor to close the file... Vim: Error reading input, exiting...        
Vim: Finished.

error: There was a problem with the editor 'vi'.

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign)
$ git status
On branch ft/home-page-redesign
Your branch is up to date with 'origin/ft/home-page-redesign'.

nothing to commit, working tree clean

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git checkout ft/home-page-redesign
Switched to branch 'ft/home-page-redesign'
Your branch is up to date with 'origin/ft/home-page-redesign'.

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign)
$ git add .

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign)
$ git commit -m "chnaged readme"
[ft/home-page-redesign 3db116b] chnaged readme
 1 file changed, 905 insertions(+), 1 deletion(-)

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 6.62 KiB | 2.21 MiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/Nkaka23dev/Gym-Git-Exercise-Solutions.git
   92751a0..3db116b  ft/home-page-redesign -> ft/home-page-redesign

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign)
$ git rebase main
Auto-merging README.md
CONFLICT (content): Merge conflict in README.md
error: could not apply 8166db2... all changes
hint: Resolve all conflicts manually, mark them as resolved with
hint: "git add/rm <conflicted_files>", then run "git rebase --continue".
hint: You can instead skip this commit: run "git rebase --skip".
hint: To abort and get back to the state before "git rebase", run "git rebase --abort".        
Could not apply 8166db2... all changes

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign|REBASE 3/5)       
$ # Gym Git Exercise Solutions 

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign|REBASE 3/5)       
$

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign|REBASE 3/5)       
$ ..This is the GYM exercises for the GYM Rwanda.
bash: ..This: command not found

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign|REBASE 3/5)       
$

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign|REBASE 3/5)       


TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign|REBASE 3/5)       
$

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign|REBASE 3/5)       
$ ### exercises 1

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign|REBASE 3/5)       
$

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign|REBASE 3/5)       
$ ...
bash: ...: command not found

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign|REBASE 3/5)       
$

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign|REBASE 3/5)       
$ TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises
bash: TheGym@DESKTOP-0FJL824: command not found

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign|REBASE 3/5)       
$ $ git init
bash: $: command not found

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign|REBASE 3/5)       
$ Initialized empty Git repository in C:/Users/TheGym/Desktop/gitExercises/.git/
bash: Initialized: command not found


TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign|REBASE 3/5)       
$

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign|REBASE 3/5)       
$ TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (master)
bash: syntax error near unexpected token `('

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign|REBASE 3/5)       
$ $ git branch -M main
bash: $: command not found

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign|REBASE 3/5)       
$

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign|REBASE 3/5)       
$ TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
bash: syntax error near unexpected token `('

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign|REBASE 3/5)       
$ $ git status
bash: $: command not found

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign|REBASE 3/5)       
$ On branch main
bash: On: command not found

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign|REBASE 3/5)       
$

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign|REBASE 3/5)       
$ No commits yet
bash: No: command not found

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign|REBASE 3/5)       
$

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign|REBASE 3/5)
$ Untracked files:
bash: Untracked: command not found

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign|REBASE 3/5)       
$   (use "git add <file>..." to include in what will be committed)
bash: use: command not found

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign|REBASE 3/5)       
$         README.md
bash: README.md: command not found

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign|REBASE 3/5)       
$

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign|REBASE 3/5)       
$ nothing added to commit but untracked files present (use "git add" to track)
bash: syntax error near unexpected token `('

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign|REBASE 3/5)       
$

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign|REBASE 3/5)       
$ TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
bash: syntax error near unexpected token `('

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign|REBASE 3/5)       
$ $ git add .
bash: $: command not found

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign|REBASE 3/5)       
$


TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign|REBASE 3/5)
$ git reabse main
git: 'reabse' is not a git command. See 'git --help'.

The most similar command is
        rebase

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign|REBASE 3/5)       
$ git rebase main
fatal: It seems that there is already a rebase-merge directory, and
I wonder if you are in the middle of another rebase.  If that is the
case, please try
        git rebase (--continue | --abort | --skip)
If that is not the case, please
        rm -fr ".git/rebase-merge"
and run me again.  I am stopping in case you still have something
valuable there.


TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign|REBASE 3/5)       
$ git add/rm README.md
git: 'add/rm' is not a git command. See 'git --help'.

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign|REBASE 3/5)       
$ git rebase --abort

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign)
$ git status
On branch ft/home-page-redesign
Your branch is up to date with 'origin/ft/home-page-redesign'.

nothing to commit, working tree clean

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign)
$ git merge main
Merge made by the 'ort' strategy.
 home.html     |  1 +
 services.html |  5 +++++
 team.html     | 14 ++++++++++++++
 3 files changed, 20 insertions(+)
 create mode 100644 team.html

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign)
$ git status
On branch ft/home-page-redesign
Your branch is ahead of 'origin/ft/home-page-redesign' by 12 commits.

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)  

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git push
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/Nkaka23dev/Gym-Git-Exercise-Solutions.git
   d06de9f..02fd0e1  main -> main

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git branch
  dev
  ft/bundle-2    
  ft/contact-page
  ft/faq-page    
  ft/home-page-redesign
  ft/service-redesign
  ft/team-page
* main

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git checkout
Your branch is up to date with 'origin/main'.

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git checkout  ft/home-page-redesign
Switched to branch 'ft/home-page-redesign'
Your branch is up to date with 'origin/ft/home-page-redesign'.

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign)
$ git merge main
Already up to date.

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   home.html

no changes added to commit (use "git add" and/or "git commit -a")

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git add .

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git commit -m "added  content with style s"
[main 5b86392] added  content with style s
 1 file changed, 2 insertions(+)

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (main)
$ git checkout ft/home-page-redesign
Switched to branch 'ft/home-page-redesign'
Your branch is up to date with 'origin/ft/home-page-redesign'.

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign)
$ git rebase main
Auto-merging README.md
CONFLICT (content): Merge conflict in README.md
error: could not apply 8166db2... all changes
hint: Resolve all conflicts manually, mark them as resolved with
hint: "git add/rm <conflicted_files>", then run "git rebase --continue".
hint: You can instead skip this commit: run "git rebase --skip".
hint: To abort and get back to the state before "git rebase", run "git rebase --abort".        
Could not apply 8166db2... all changes

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign|REBASE 3/5)       
$ git merge origin/main
Already up to date.

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign|REBASE 3/5)       
$ git push
fatal: You are not currently on a branch.
To push the history leading to the current (detached HEAD)
state now, use

    git push origin HEAD:<name-of-remote-branch>


TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign|REBASE 3/5)       
$ git push origin HEAD:main
Enumerating objects: 11, done.
Counting objects: 100% (11/11), done.
Delta compression using up to 4 threads
Compressing objects: 100% (9/9), done.
Writing objects: 100% (9/9), 1.14 KiB | 584.00 KiB/s, done.
Total 9 (delta 4), reused 0 (delta 0), pack-reused 0

E325: ATTENTION
Found a swap file by the name "~/Desktop/gitExercises/.git/.COMMIT_EDITMSG.swp"
          owned by: TheGym   dated: Thu Nov 10 12:25:12 2022
         file name: ~TheGym/Desktop/gitExercises/.git/COMMIT_EDITMSG
          modified: YES
         user name: TheGym   host name: DESKTOP-0FJL824
remote: Resolving deltas: 100% (4/4), completed with 1 local object.
To https://github.com/Nkaka23dev/Gym-Git-Exercise-Solutions.git
   02fd0e1..266fb5c  HEAD -> main

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign|REBASE 3/5)       
$ git rebase main
fatal: It seems that there is already a rebase-merge directory, and
I wonder if you are in the middle of another rebase.  If that is the
case, please try
        git rebase (--continue | --abort | --skip)
If that is not the case, please
        rm -fr ".git/rebase-merge"
and run me again.  I am stopping in case you still have something
valuable there.


TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign|REBASE 3/5)       
$ git rebase --continue
hint: Waiting for your editor to close the file... Vim: Error reading input, exiting...        
Vim: Finished.

error: There was a problem with the editor 'vi'.
Please supply the message using either -m or -F option.

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign|REBASE 3/5)       
$ git rebase --abort

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign)
$ git rebase main
Auto-merging README.md
CONFLICT (content): Merge conflict in README.md
error: could not apply 8166db2... all changes
hint: Resolve all conflicts manually, mark them as resolved with
hint: "git add/rm <conflicted_files>", then run "git rebase --continue".
hint: You can instead skip this commit: run "git rebase --skip".
hint: To abort and get back to the state before "git rebase", run "git rebase --abort".        
Could not apply 8166db2... all changes

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign|REBASE 3/5)       
$ git diff

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign|REBASE 3/5)
$ git status
interactive rebase in progress; onto 5b86392
Last commands done (3 commands done):
   pick 8473371 created faq pages
   pick 8166db2 all changes
  (see more in file .git/rebase-merge/done)
Next commands to do (2 remaining commands):
   pick 92751a0 all changes
   pick 3db116b chnaged readme
  (use "git rebase --edit-todo" to view and edit)
You are currently rebasing branch 'ft/home-page-redesign' on '5b86392'.
  (all conflicts fixed: run "git rebase --continue")

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   README.md


TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign|REBASE 3/5)       
$ git rebase --abort

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign)
$ git diff main
diff --git a/contact.html b/contact.html
new file mode 100644
index 0000000..2ea9fb8
--- /dev/null
+++ b/contact.html
@@ -0,0 +1,12 @@
+<!DOCTYPE html>
+<html lang="en">
+<head>
+    <meta charset="UTF-8">
+    <meta http-equiv="X-UA-Compatible" content="IE=edge">
+    <meta name="viewport" content="width=device-width, initial-scale=1.0">
+    <title>Contact Page</title>
+</head>
+<body>
+   <h1>Contact Page .................</h1> 
+</body>
+</html>

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign)
$ git rebase main
Auto-merging README.md
CONFLICT (content): Merge conflict in README.md
error: could not apply 8166db2... all changes
hint: Resolve all conflicts manually, mark them as resolved with
hint: "git add/rm <conflicted_files>", then run "git rebase --continue".
hint: You can instead skip this commit: run "git rebase --skip".
hint: To abort and get back to the state before "git rebase", run "git rebase --abort".        
Could not apply 8166db2... all changes

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign|REBASE 3/5)       
$ git add .

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign|REBASE 3/5)       
$ git commit -m "fix: solved rebase conflicts"
[detached HEAD 4df28fa] fix: solved rebase conflicts
 1 file changed, 2 insertions(+)

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign|REBASE 3/5)       
$ git rebase main
fatal: It seems that there is already a rebase-merge directory, and
I wonder if you are in the middle of another rebase.  If that is the
case, please try
        git rebase (--continue | --abort | --skip)
If that is not the case, please
        rm -fr ".git/rebase-merge"
and run me again.  I am stopping in case you still have something
valuable there.


TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign|REBASE 3/5)       
$ git rebase --continue
Auto-merging README.md
CONFLICT (content): Merge conflict in README.md
error: could not apply 92751a0... all changes
hint: Resolve all conflicts manually, mark them as resolved with
hint: "git add/rm <conflicted_files>", then run "git rebase --continue".
hint: You can instead skip this commit: run "git rebase --skip".
hint: To abort and get back to the state before "git rebase", run "git rebase --abort".        
Could not apply 92751a0... all changes

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign|REBASE 4/5)       
$ git add .

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign|REBASE 4/5)       
$ git commit -m "fix: solving rebase error"
[detached HEAD 5c9db35] fix: solving rebase error
 1 file changed, 3 insertions(+)

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign|REBASE 4/5)       
$ git rebase --continue
Auto-merging README.md
CONFLICT (content): Merge conflict in README.md
error: could not apply 3db116b... chnaged readme
hint: Resolve all conflicts manually, mark them as resolved with
hint: "git add/rm <conflicted_files>", then run "git rebase --continue".
hint: You can instead skip this commit: run "git rebase --skip".
hint: To abort and get back to the state before "git rebase", run "git rebase --abort".        
Could not apply 3db116b... chnaged readme

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign|REBASE 5/5)       
$ git add .

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign|REBASE 5/5)       
$ git commit -m "fix: solving rebase error"
[detached HEAD 752011a] fix: solving rebase error
 1 file changed, 2 insertions(+), 4 deletions(-)

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign|REBASE 5/5)       
$ git rebase --continue
Successfully rebased and updated refs/heads/ft/home-page-redesign.

TheGym@DESKTOP-0FJL824 MINGW64 ~/Desktop/gitExercises (ft/home-page-redesign)
$
...
