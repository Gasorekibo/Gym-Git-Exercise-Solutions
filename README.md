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

```
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
```