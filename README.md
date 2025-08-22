# git-cafe-exercise
# Bundle 6

```bash
PS D:\old\The Gym\git-exercises\fork> git clone https://github.com/ishluc12/git-cafe-exercise.git
Cloning into 'git-cafe-exercise'...
remote: Enumerating objects: 107, done.
remote: Counting objects: 100% (15/15), done.
remote: Compressing objects: 100% (11/11), done.
remote: Total 107 (delta 5), reused 4 (delta 4), pack-reused 92 (from 1)
Receiving objects: 100% (107/107), 1.95 MiB | 115.00 KiB/s, done.
Resolving deltas: 100% (5/5), done.
PS D:\old\The Gym\git-exercises\fork> git add --all
warning: adding embedded git repository: fork/git-cafe-exercise
hint: You've added another git repository inside your current repository.
hint: Clones of the outer repository will not contain the contents of
hint: the embedded repository and will not know how to obtain it.
hint: If you meant to add a submodule, use:
hint:
hint:   git submodule add <url> fork/git-cafe-exercise
hint:
hint: If you added this path by mistake, you can remove it from the
hint: index with:
hint:
hint:   git rm --cached fork/git-cafe-exercise
hint:
hint: See "git help submodule" for more information.
hint: Disable this message with "git config set advice.addEmbeddedRepo false"
PS D:\old\The Gym\git-exercises\fork> git remote -v
git-copy        https://github.com/ishluc12/Git-exercise2.git (fetch)
git-copy        https://github.com/ishluc12/Git-exercise2.git (push)
origin  https://github.com/ishluc12/Git-Exercise.git (fetch)
origin  https://github.com/ishluc12/Git-Exercise.git (push)
PS D:\old\The Gym\git-exercises\fork> cd .\git-cafe-exercise\
PS D:\old\The Gym\git-exercises\fork\git-cafe-exercise> git status   
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   index.html

no changes added to commit (use "git add" and/or "git commit -a")
PS D:\old\The Gym\git-exercises\fork\git-cafe-exercise> git add --all
PS D:\old\The Gym\git-exercises\fork\git-cafe-exercise> git commit -m "i have added changes to the index file"
[main f1a98ee] i have added changes to the index file
 1 file changed, 286 insertions(+), 226 deletions(-)
PS D:\old\The Gym\git-exercises\fork\git-cafe-exercise> git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 1.41 KiB | 480.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/ishluc12/git-cafe-exercise.git
   d1d3f9c..f1a98ee  main -> main
PS D:\old\The Gym\git-exercises\fork\git-cafe-exercise> git status 
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean
PS D:\old\The Gym\git-exercises\fork\git-cafe-exercise> git branch
* main
PS D:\old\The Gym\git-exercises\fork\git-cafe-exercise> git checkout -b ft/menu     
Switched to a new branch 'ft/menu'
PS D:\old\The Gym\git-exercises\fork\git-cafe-exercise> git add menu.html
PS D:\old\The Gym\git-exercises\fork\git-cafe-exercise> git commit -m "creating menu page"    
[ft/menu a1e7601] creating menu page
 1 file changed, 14 insertions(+)
 create mode 100644 menu.html
PS D:\old\The Gym\git-exercises\fork\git-cafe-exercise> git pudh
git: 'pudh' is not a git command. See 'git --help'.

The most similar command is
        push
PS D:\old\The Gym\git-exercises\fork\git-cafe-exercise> git push
fatal: The current branch ft/menu has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/menu

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

PS D:\old\The Gym\git-exercises\fork\git-cafe-exercise> git push --set-upstream origin ft/menu
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 447 bytes | 74.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/menu' on GitHub by visiting:
remote:      https://github.com/ishluc12/git-cafe-exercise/pull/new/ft/menu
remote:
To https://github.com/ishluc12/git-cafe-exercise.git
 * [new branch]      ft/menu -> ft/menu
branch 'ft/menu' set up to track 'origin/ft/menu'.
PS D:\old\The Gym\git-exercises\fork\git-cafe-exercise> git checkout main                     
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
PS D:\old\The Gym\git-exercises\fork\git-cafe-exercise> git checkout -b ft/bug-fix
Switched to a new branch 'ft/bug-fix'
PS D:\old\The Gym\git-exercises\fork\git-cafe-exercise> git add contact.html 
PS D:\old\The Gym\git-exercises\fork\git-cafe-exercise> git commit -m "renaming index-4.html to contact.hml"
[ft/bug-fix 1a886bd] renaming index-4.html to contact.hml
 1 file changed, 204 insertions(+)
 create mode 100644 contact.html
PS D:\old\The Gym\git-exercises\fork\git-cafe-exercise> git push
fatal: The current branch ft/bug-fix has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/bug-fix

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

PS D:\old\The Gym\git-exercises\fork\git-cafe-exercise> git push --set-upstream origin ft/bug-fix
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 2.50 KiB | 426.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/bug-fix' on GitHub by visiting:
remote:      https://github.com/ishluc12/git-cafe-exercise/pull/new/ft/bug-fix
remote:
To https://github.com/ishluc12/git-cafe-exercise.git
 * [new branch]      ft/bug-fix -> ft/bug-fix
branch 'ft/bug-fix' set up to track 'origin/ft/bug-fix'.
PS D:\old\The Gym\git-exercises\fork\git-cafe-exercise> git add .
PS D:\old\The Gym\git-exercises\fork\git-cafe-exercise> git commit -m "changing telephone number to +1 800 659 6035"
[ft/bug-fix a6fc2b1] changing telephone number to +1 800 659 6035
 2 files changed, 171 insertions(+), 360 deletions(-)
 delete mode 100644 index-4.html
PS D:\old\The Gym\git-exercises\fork\git-cafe-exercise> git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 1.19 KiB | 1.19 MiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/ishluc12/git-cafe-exercise.git
   1a886bd..a6fc2b1  ft/bug-fix -> ft/bug-fix
PS D:\old\The Gym\git-exercises\fork\git-cafe-exercise> 
```
