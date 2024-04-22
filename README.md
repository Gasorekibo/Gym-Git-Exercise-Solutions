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

### Exercise 2

```bash
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git checkout main
Switched to branch 'main'
Your branch is behind 'origin/main' by 8 commits, and can be fast-forwarded.
  (use "git pull" to update your local branch)
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git pull
Updating 2406b7b..6e6f59e
Fast-forward
 README.md     | 160 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 about.html    |  11 ++++
 home.html     |  11 ++++
 services.html |  11 ++++
 4 files changed, 193 insertions(+)
 create mode 100644 README.md
 create mode 100644 about.html
 create mode 100644 services.html
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git checkout -b ft/service-redesign
Switched to a new branch 'ft/service-redesign'
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git add .
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git commit -m "update services"
[ft/service-redesign fb3b9b1] update services
 1 file changed, 13 insertions(+), 7 deletions(-)
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git push
fatal: The current branch ft/service-redesign has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/service-redesign

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git push --set-upstream origin ft/service-redesign
Writing objects: 100% (3/3), 563 bytes | 563.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/service-redesign' on GitHub by visiting:
remote:      https://github.com/Gasorekibo/Gym-Git-Exercise-Solutions/pull/new/ft/service-redesign
remote:
To https://github.com/Gasorekibo/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/service-redesign -> ft/service-redesign
branch 'ft/service-redesign' set up to track 'origin/ft/service-redesign'.
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git add .
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git commit -m "creating merge conflict"
[main 15d62ab] creating merge conflict
 1 file changed, 5 insertions(+)
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 520 bytes | 520.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/Gasorekibo/Gym-Git-Exercise-Solutions.git
   6e6f59e..15d62ab  main -> main
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git checkout ft/service-redesign
Switched to branch 'ft/service-redesign'
Your branch is up to date with 'origin/ft/service-redesign'.
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git diff
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git merge ft/service-redesign
Auto-merging services.html
CONFLICT (content): Merge conflict in services.html
Automatic merge failed; fix conflicts and then commit the result.
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git diff
diff --cc services.html
index 4b3eeec,0fcbc77..0000000
--- a/services.html
+++ b/services.html
@@@ -1,16 -1,17 +1,27 @@@
  <!DOCTYPE html>
  <html lang="en">
- <head>
-     <meta charset="UTF-8">
-     <meta name="viewport" content="width=device-width, initial-scale=1.0">
+   <head>
+     <meta charset="UTF-8" />
+     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
      <title>Git & GitHub</title>
- </head>
- <body>
+   </head>
+   <body>
      <h1>Services page</h1>
++<<<<<<< HEAD
 +    <h5>Adding new services from main branch</h5>
 +    <ul>
 +        <li>Git: Fast version control system.</li>
 +        <li>SEO: Optimize your website</li>
 +    </ul>
 +</body>
- </html>
++</html>
++=======
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git checkout ft/service-redesign
error: you need to resolve your current index first
services.html: needs merge
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git merge main               
error: Merging is not possible because you have unmerged files.
hint: Fix them up in the work tree, and then use 'git add/rm <file>'
hint: as appropriate to mark resolution and make a commit.
fatal: Exiting because of an unresolved conflict.
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git diff
diff --cc services.html
index 4b3eeec,0fcbc77..0000000
--- a/services.html
+++ b/services.html
@@@ -1,16 -1,17 +1,27 @@@
  <!DOCTYPE html>
  <html lang="en">
- <head>
-     <meta charset="UTF-8">
-     <meta name="viewport" content="width=device-width, initial-scale=1.0">
+   <head>
+     <meta charset="UTF-8" />
+     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
      <title>Git & GitHub</title>
- </head>
- <body>
+   </head>
+   <body>
      <h1>Services page</h1>
++<<<<<<< HEAD
 +    <h5>Adding new services from main branch</h5>
 +    <ul>
 +        <li>Git: Fast version control system.</li>
 +        <li>SEO: Optimize your website</li>
 +    </ul>
diff --cc services.html
index 4b3eeec,0fcbc77..0000000
--- a/services.html
+++ b/services.html
@@@ -1,16 -1,17 +1,27 @@@
  <!DOCTYPE html>
  <html lang="en">
- <head>
-     <meta charset="UTF-8">
-     <meta name="viewport" content="width=device-width, initial-scale=1.0">
+   <head>
+     <meta charset="UTF-8" />
+     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
      <title>Git & GitHub</title>
- </head>
- <body>
+   </head>
+   <body>
      <h1>Services page</h1>
++<<<<<<< HEAD
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git diff
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git commit -a -m "solved merge conflict"
[main 1f40197] solved merge conflict
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git push
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 352 bytes | 352.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/Gasorekibo/Gym-Git-Exercise-Solutions.git
   15d62ab..1f40197  main -> main
```


## Bundle 3

### Exercise 1

``` bash
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git branch
  dev
  ft/bundle-2
  ft/service-redesign
* main
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git checkout -b ft/team-page
Switched to a new branch 'ft/team-page'
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git add .
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git commit -m "add team page"
[ft/team-page 1537e3a] add team page
 1 file changed, 11 insertions(+)
 create mode 100644 team.html
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git push
fatal: The current branch ft/team-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/team-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git push --set-upstream origin ft/team-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 436 bytes | 218.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/team-page' on GitHub by visiting:
remote:      https://github.com/Gasorekibo/Gym-Git-Exercise-Solutions/pull/new/ft/team-page       
remote:
To https://github.com/Gasorekibo/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/team-page -> ft/team-page
branch 'ft/team-page' set up to track 'origin/ft/team-page'.
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git checkout -b ft/contact-page
Switched to a new branch 'ft/contact-page'
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git checkout ft/team-page
Switched to branch 'ft/team-page'
Your branch is up to date with 'origin/ft/team-page'.
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git log
commit 1537e3abe4210c31e0c9adf5eb7745174163d968 (HEAD -> ft/team-page, origin/ft/team-page)
Author: Gasorekibo <m.gasore@alustudent.com>
Date:   Mon Apr 22 17:48:40 2024 +0200

    add team page

commit 0f5d903d02ffe0150438269a98ef0168049c6e0e (origin/main, main, ft/contact-page)
Author: Gasorekibo <m.gasore@alustudent.com>
Date:   Mon Apr 22 16:29:59 2024 +0200

    add answer to README file

commit 1f40197a5e1e472b9d99423d4b5d1190dcce7c03
Merge: 15d62ab fb3b9b1
Author: Gasorekibo <m.gasore@alustudent.com>
Date:   Mon Apr 22 16:24:12 2024 +0200

    solved merge conflict

commit 15d62abc1af81509305001452f15912f40e00c31
Author: Gasorekibo <m.gasore@alustudent.com>
Date:   Mon Apr 22 16:05:47 2024 +0200

    creating merge conflict

commit fb3b9b1fa0b908a82db0fcdaa4e844b47782ecaf (origin/ft/service-redesign, ft/service-redesign)
Author: Gasorekibo <m.gasore@alustudent.com>
Date:   Mon Apr 22 15:59:57 2024 +0200

    update services

PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git checkout contact-page
error: pathspec 'contact-page' did not match any file(s) known to git      
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git checkout ft/contact-page
Switched to branch 'ft/contact-page'
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git cherry-pick 1537e3abe4210c31e0c9adf5eb7745174163d968
[ft/contact-page 273871a] add team page
 Date: Mon Apr 22 17:48:40 2024 +0200
 1 file changed, 11 insertions(+)
 create mode 100644 team.html
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git add .
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git commit -m "added contact page"
[ft/contact-page 3cc807a] added contact page
 1 file changed, 11 insertions(+)
 create mode 100644 contact.html
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git push
fatal: The current branch ft/contact-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/contact-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git push --set-upstream origin ft/contact-page
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 8 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 680 bytes | 680.00 KiB/s, done.
Total 6 (delta 3), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (3/3), completed with 1 local object.       
remote:
remote: Create a pull request for 'ft/contact-page' on GitHub by visiting: 
remote:      https://github.com/Gasorekibo/Gym-Git-Exercise-Solutions/pull/new/ft/contact-page
remote:
To https://github.com/Gasorekibo/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/contact-page -> ft/contact-page
branch 'ft/contact-page' set up to track 'origin/ft/contact-page'.
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git checkout ft/contact-page
Already on 'ft/contact-page'
Your branch is up to date with 'origin/ft/contact-page'.
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git checkout -b ft/faq-page
Switched to a new branch 'ft/faq-page'
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git add .
Revert "add team page"
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git commit -m "created faq page"
[ft/faq-page 5cc73e1] created faq page
 1 file changed, 11 insertions(+)
 create mode 100644 faq.html
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git push        
fatal: The current branch ft/faq-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/faq-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git push --set-upstream origin ft/faq-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/faq-page' on GitHub by visiting:
remote:      https://github.com/Gasorekibo/Gym-Git-Exercise-Solutions/pull/new/ft/faq-page
remote:
To https://github.com/Gasorekibo/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/faq-page -> ft/faq-page
branch 'ft/faq-page' set up to track 'origin/ft/faq-page'.
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git revert 1537e3abe4210c31e0c9adf5eb7745174163d968
[ft/faq-page 01c413d] Revert "add team page"
 1 file changed, 11 deletions(-)
 delete mode 100644 team.html
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git add .
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git commit -m "revert change"
On branch ft/faq-page
Your branch is ahead of 'origin/ft/faq-page' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises> git push
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 292 bytes | 292.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/Gasorekibo/Gym-Git-Exercise-Solutions.git
   5cc73e1..01c413d  ft/faq-page -> ft/faq-page
PS C:\Users\Lenovo\OneDrive\Desktop\The Gym\Git Exercises>
```