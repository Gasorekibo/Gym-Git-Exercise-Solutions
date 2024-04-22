# GIT Exercises

## Bundle 1

### Exercise 1

```bash
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git init
Initialized empty Git repository in C:/Users/Lenovo/OneDrive/Desktop/The Gym/Git Exercises/.git/
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git branch -m master main       
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git add .
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git commit -m "bundle 1 exercises one"
[main (root-commit) 2406b7b] bundle 1 exercises one
 1 file changed, 11 insertions(+)
 create mode 100644 index.html
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git remote add origin https://github.com/Gasorekibo/Gym-Git-Exercise-Solutions.git
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git branch -M main
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git push -u origin main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 398 bytes | 199.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/Gasorekibo/Gym-Git-Exercise-Solutions.git
 * [new branch]      main -> main
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git checkout -b dev
Switched to a new branch 'dev'
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git checkout test
error: pathspec 'test' did not match any file(s) known to git
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git checkout -b test
Switched to a new branch 'test'
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git checkout dev
Switched to branch 'dev'
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git branch -d test
Deleted branch test (was 2406b7b).
```


### Exercise 2

```bash
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git add .\home.html
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git stash
Saved working directory and index state WIP on dev: e3166e9 delete some files
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git add .\about.html
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git stash
Saved working directory and index state WIP on dev: e3166e9 delete some files
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git add .\team.html
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git stash
Saved working directory and index state WIP on dev: e3166e9 delete some files
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git stash list
stash@{0}: WIP on dev: e3166e9 delete some files
stash@{1}: WIP on dev: e3166e9 delete some files
stash@{2}: WIP on dev: e3166e9 delete some files
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git stash pop 1
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

Dropped refs/stash@{1} (cd889b0d472d7b9fa8951c6c043031dea465d729)
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git stash list
stash@{0}: WIP on dev: e3166e9 delete some files
stash@{1}: WIP on dev: e3166e9 delete some files
git stash pop 1
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   home.html

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

Dropped refs/stash@{1} (c098a251b9695d626ad1710bcbc3c7e4e4b5186e)
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git stash list
stash@{0}: WIP on dev: e3166e9 delete some files
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git add .
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git commit -m "done with git stash exercises"
[dev 8b68eda] done with git stash exercises
 3 files changed, 70 insertions(+)
 create mode 100644 about.html
 create mode 100644 home.html
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git push
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 8 threads
Compressing objects: 100% (5/5), done.
Writing objects: 100% (5/5), 1.64 KiB | 1.64 MiB/s, done.
Total 5 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/Gasorekibo/Gym-Git-Exercise-Solutions.git
   e3166e9..8b68eda  dev -> dev
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git stash list
stash@{0}: WIP on dev: e3166e9 delete some files
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git stash pop
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

Dropped refs/stash@{0} (138b302588a3dd0a03a859d46e80d3f10af02070)
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git reset --hard
HEAD is now at 8b68eda done with git stash exercises
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git status
On branch dev
Your branch is up to date with 'origin/dev'.

nothing to commit, working tree clean
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git stash list
```

# Bundle 2

### Exercise 1

```bash
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git branch
* dev
  main
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git checkout -b ft/bundle-2
Switched to a new branch 'ft/bundle-2'
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git add .
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git commit -m "pull request against main"
[ft/bundle-2 8f00242] pull request against main
 2 files changed, 12 insertions(+), 1 deletion(-)
 create mode 100644 services.html
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git push
fatal: The current branch ft/bundle-2 has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/bundle-2

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git push --set-upstream origin ft/bundle-2
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 8 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 593 bytes | 593.00 KiB/s, done.
Total 4 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote:      https://github.com/Gasorekibo/Gym-Git-Exercise-Solutions/pull/new/ft/bundle-2
remote: 
To https://github.com/Gasorekibo/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/bundle-2 -> ft/bundle-2
branch 'ft/bundle-2' set up to track 'origin/ft/bundle-2'.
```