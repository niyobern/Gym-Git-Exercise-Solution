# Git Exercises

## Bundle 1

### Exercise 1

``` bash
git init
Initialized empty Git repository in C:/Users/SICHA/Desktop/Gym/.git/
git branch -a

git add .

git commit -m "added README file"
[main (root-commit) 1e5903b] added README file
 1 file changed, 4 insertions(+)
git branch -a
* main
git branch -m master

git branch -a
* master
git branch -m main && git branch -a
* main
git remote add origin https://github.com/niyobern/Gym-Git-exercise-Solution.git

git push origin main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 2 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 311 bytes | 44.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
remote: This repository moved. Please use the new location:
remote:   https://github.com/niyobern/Gym-Git-Exercise-Solution.git
To https://github.com/niyobern/Gym-Git-exercise-Solution.git
 * [new branch]      main -> main
git branch dev

git switch dev
Switched to branch 'dev'
M       README.md
git branch test

git branch -d test
Deleted branch test (was 1e5903b).
```

### Exercises 2

``` bash
C:\Users\bernard\documents\Gym\git>git status
On branch main
Your branch is up to date with 'origin/main'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        home.html

nothing added to commit but untracked files present (use "git add" to track)

C:\Users\bernard\documents\Gym\git>git stash -u save "home"
fatal: subcommand wasn't specified; 'push' can't be assumed due to unexpected token 'save'

C:\Users\bernard\documents\Gym\git>git stash save "home" -u
Saved working directory and index state On main: home

C:\Users\bernard\documents\Gym\git>git stash "about" -u
fatal: subcommand wasn't specified; 'push' can't be assumed due to unexpected token 'about'

C:\Users\bernard\documents\Gym\git>git stash save "about" -u
Saved working directory and index state On main: about

C:\Users\bernard\documents\Gym\git>git stash save "team" -u
Saved working directory and index state On main: team

C:\Users\bernard\documents\Gym\git>git stash list
stash@{0}: On main: team
stash@{1}: On main: about
stash@{2}: On main: home

C:\Users\bernard\documents\Gym\git>git stash pop stash@{1}
Already up to date.
On branch main
Your branch is up to date with 'origin/main'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        about.html

nothing added to commit but untracked files present (use "git add" to track)
Dropped stash@{1} (130bebee01954a414b0e8820f9e96b1fcd711b60)

C:\Users\bernard\documents\Gym\git>git stash list
stash@{0}: On main: team
stash@{1}: On main: home

C:\Users\bernard\documents\Gym\git>git stash pop stash@{1}
Already up to date.
On branch main
Your branch is up to date with 'origin/main'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        about.html
        home.html

nothing added to commit but untracked files present (use "git add" to track)
Dropped stash@{1} (a8fad0d2421a6e4c615431398b935ff3cc5ccb60)

C:\Users\bernard\documents\Gym\git>git add .

C:\Users\bernard\documents\Gym\git>git commit -m "comiting home and about"
[main 8a9d2c4] comiting home and about
 2 files changed, 20 insertions(+)
 create mode 100644 about.html
 create mode 100644 home.html

C:\Users\bernard\documents\Gym\git>git push origin main
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 2 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 454 bytes | 30.00 KiB/s, done.
Total 4 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), done.
To https://github.com/niyobern/Gym-Git-Exercise-Solution
   3b0b96c..8a9d2c4  main -> main

C:\Users\bernard\documents\Gym\git>git stash list
stash@{0}: On main: team

C:\Users\bernard\documents\Gym\git>git stash pop stash@{0}
Already up to date.
On branch main
Your branch is up to date with 'origin/main'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        team.html

nothing added to commit but untracked files present (use "git add" to track)
Dropped stash@{0} (2b158be2ad7f18014d4b54e1aac742be3594406e)

C:\Users\bernard\documents\Gym\git>git reset --hard
HEAD is now at 8a9d2c4 comiting home and about

C:\Users\bernard\documents\Gym\git>git branch list

C:\Users\bernard\documents\Gym\git>git branch
  list
* main

C:\Users\bernard\documents\Gym\git>git branch -d list
Deleted branch list (was 8a9d2c4).
```
## Bundle 2

### Exercise 1

``` bash
C:\Users\bernard\documents\Gym\git>git branch ft/bundle-2
C:\Users\bernard\documents\Gym\git>git switch ft/bundle-2
C:\Users\bernard\documents\Gym\git>git add .
C:\Users\bernard\documents\Gym\git>git commit -m "adding the services.html"
[ft/bundle-2 6608c47] adding the services.html
 1 file changed, 10 insertions(+)
 create mode 100644 services.html
C:\Users\bernard\documents\Gym\git>git push origin ft/bundle-2
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 2 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 367 bytes | 52.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote:      https://github.com/niyobern/Gym-Git-Exercise-Solution/pull/new/ft/bundle-2
remote:
To https://github.com/niyobern/Gym-Git-Exercise-Solution
 * [new branch]      ft/bundle-2 -> ft/bundle-2
C:\Users\bernard\documents\Gym\git>git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
C:\Users\bernard\documents\Gym\git>git merge ft/bundle-2
Merge made by the 'ort' strategy.
 services.htm | 10 ++++++++++
 1 file changed, 10 insertions(+)
 create mode 100644 services.html
C:\Users\bernard\documents\Gym\git>git push origin main
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 2 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 300 bytes | 60.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/niyobern/Gym-Git-Exercise-Solution
   f02d565..edbb869  main -> main
C:\Users\bernard\documents\Gym\git>
```

### Exercise 2

``` bash
C:\Users\bernard\documents\Gym\git>git checkout main
Already on 'main'
Your branch is up to date with 'origin/main'.
C:\Users\bernard\documents\Gym\git>git checkout -b ft/service-redesign
Switched to a new branch 'ft/service-redesign'
C:\Users\bernard\documents\Gym\git>git add . && git commit -m "commiting my changes to services.html"
[ft/service-redesign 637feee] commiting my changes to services.html
 1 file changed, 1 insertion(+), 1 deletion(-)
C:\Users\bernard\documents\Gym\git>git push origin ft/service-redesign
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 2 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 320 bytes | 45.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
remote:
remote: Create a pull request for 'ft/service-redesign' on GitHub by visiting:
remote:      https://github.com/niyobern/Gym-Git-Exercise-Solution/pull/new/ft/service-redesign
remote:
To https://github.com/niyobern/Gym-Git-Exercise-Solution
 * [new branch]      ft/service-redesign -> ft/service-redesign
C:\Users\bernard\documents\Gym\git>git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
C:\Users\bernard\documents\Gym\git>git add . && git commit -m "adding changes made form the main branch" && git push origin main
[main db29df2] adding changes made form the main branch
 1 file changed, 1 insertion(+), 1 deletion(-)
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 2 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 328 bytes | 25.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/niyobern/Gym-Git-Exercise-Solution
   4c4a50d..db29df2  main -> main
C:\Users\bernard\documents\Gym\git>git checkout ft/service-redesign
Switched to branch 'ft/service-redesign'
C:\Users\bernard\documents\Gym\git>git diff main ft/service-redesign
diff --git a/services.html b/services.html
index 74e3527..5d527ad 100644
--- a/services.html
+++ b/services.html
@@ -4,7 +4,7 @@
     </head>
     <body>
         <header></header>
-        <main>Changes to this page from main</main>
+        <main>New Changes to this page</main>
         <footer></footer>
     </body>
 </html>
\ No newline at end of file
C:\Users\bernard\documents\Gym\git>git merge main ft/service-redesign
Auto-merging services.html
CONFLICT (content): Merge conflict in services.html
Automatic merge failed; fix conflicts and then commit the result.
C:\Users\bernard\documents\Gym\git>git push origin main
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 2 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 361 bytes | 72.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/niyobern/Gym-Git-Exercise-Solution
   db29df2..c0d2165  main -> main
C:\Users\bernard\documents\Gym\git>
```
## Bundle 3

### Exercise 1

``` bash
C:\Users\bernard\documents\Gym\git>git checkout -b ft/team-page
Switched to a new branch 'ft/team-page'
C:\Users\bernard\documents\Gym\git>git add . && git commit -m "new team page"
[ft/team-page 3270382] new team page
 1 file changed, 10 insertions(+)
 create mode 100644 team.html
C:\Users\bernard\documents\Gym\git>git push origin ft/team-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 2 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 353 bytes | 70.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/team-page' on GitHub by visiting:
remote:      https://github.com/niyobern/Gym-Git-Exercise-Solution/pull/new/ft/team-page
remote:
To https://github.com/niyobern/Gym-Git-Exercise-Solution
 * [new branch]      ft/team-page -> ft/team-page
C:\Users\bernard\documents\Gym\git>checkout main
'checkout' is not recognized as an internal or external command,
operable program or batch file.
C:\Users\bernard\documents\Gym\git>git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
C:\Users\bernard\documents\Gym\git>git branch ft/contact-page
C:\Users\bernard\documents\Gym\git>git checkout ft/team-page
Switched to branch 'ft/team-page'
C:\Users\bernard\documents\Gym\git>git>git log
commit 32703827ead060eabe055f44907b357cc6e85ba4 (HEAD -> ft/team-page, origin/ft/team-page)
Author: niyobern <niyobern@outlook.com>
Date:   Wed May 17 04:26:41 2023 +0200

    new team page
...
C:\Users\bernard\documents\Gym\git>git checkout ft/contact-page
Switched to branch 'ft/contact-page'
C:\Users\bernard\documents\Gym\git>git cherry-pick 32703827ead060eabe055f44907b357cc6e85ba4
[ft/contact-page f9549c5] new team page
 Date: Wed May 17 04:26:41 2023 +0200
 1 file changed, 10 insertions(+)
 create mode 100644 team.html
C:\Users\bernard\documents\Gym\git>git push origin ft/contact-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 2 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 357 bytes | 59.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/contact-page' on GitHub by visiting:
remote:      https://github.com/niyobern/Gym-Git-Exercise-Solution/pull/new/ft/contact-page
remote:
To https://github.com/niyobern/Gym-Git-Exercise-Solution
 * [new branch]      ft/contact-page -> ft/contact-page
C:\Users\bernard\documents\Gym\git>git branch ft/faq-page
C:\Users\bernard\documents\Gym\git>git add . && git commit -m "new faq"
[ft/contact-page b350730] new faq
 1 file changed, 11 insertions(+)
 create mode 100644 faq.html
C:\Users\bernard\documents\Gym\git>git push origin ft/faq-page
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'ft/faq-page' on GitHub by visiting:
remote:      https://github.com/niyobern/Gym-Git-Exercise-Solution/pull/new/ft/faq-page
remote:
To https://github.com/niyobern/Gym-Git-Exercise-Solution
 * [new branch]      ft/faq-page -> ft/faq-page
C:\Users\bernard\documents\Gym\git>git revert 32703827ead060eabe055f44907b357cc6e85ba4
[ft/team-page 3d33665] Revert "new team page"
 1 file changed, 10 deletions(-)
 delete mode 100644 team.html
C:\Users\bernard\documents\Gym\git>git push origin ft/team-page
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 2 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 245 bytes | 35.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/niyobern/Gym-Git-Exercise-Solution
   3270382..3d33665  ft/team-page -> ft/team-page
C:\Users\bernard\documents\Gym\git>

```
### Exercise 2

``` bash
C:\Users\Bernard\Documents\Gym>cd git

C:\Users\Bernard\Documents\Gym\git>git checkout ft/faq-page
Switched to branch 'ft/faq-page'

C:\Users\Bernard\Documents\Gym\git>git branch ft/home-page-redesign

C:\Users\Bernard\Documents\Gym\git>git switch main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

C:\Users\Bernard\Documents\Gym\git>git add home.html

C:\Users\Bernard\Documents\Gym\git>git commit -m "changes made on home.html"
[main 7f0617d] changes made on home.html
 1 file changed, 3 insertions(+), 1 deletion(-)

C:\Users\Bernard\Documents\Gym\git>git push origin main
Enumerating objects: 9, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 2 threads
Compressing objects: 100% (5/5), done.
Writing objects: 100% (5/5), 661 bytes | 82.00 KiB/s, done.
Total 5 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 1 local object.
To https://github.com/niyobern/Gym-Git-Exercise-Solution
   1756134..f2fae88  main -> main

C:\Users\Bernard\Documents\Gym\git>git checkout ft/home-page-redesign
Switched to branch 'ft/home-page-redesign'

C:\Users\Bernard\Documents\Gym\git>git rebase main
Successfully rebased and updated refs/heads/ft/home-page-redesign.

C:\Users\Bernard\Documents\Gym\git>git add .

C:\Users\Bernard\Documents\Gym\git>git commit -m "comiting on ft/home-page-redesig branch"
[ft/home-page-redesign 55717f5] comiting on ft/home-page-redesig branch
 1 file changed, 1 insertion(+)

C:\Users\Bernard\Documents\Gym\git>git push origin ft/home-page-redesign
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 2 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 716 bytes | 79.00 KiB/s, done.
Total 6 (delta 3), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (3/3), completed with 2 local objects.
remote:
remote: Create a pull request for 'ft/home-page-redesign' on GitHub by visiting:
remote:      https://github.com/niyobern/Gym-Git-Exercise-Solution/pull/new/ft/home-page-redesign
remote:
To https://github.com/niyobern/Gym-Git-Exercise-Solution
 * [new branch]      ft/home-page-redesign -> ft/home-page-redesign

C:\Users\Bernard\Documents\Gym\git>

```

## Bundle 4

### Exercise 1

``` bash

C:\Users\Bernard\Documents\Gym\git>git checkout main
Already on 'main'
Your branch is up to date with 'origin/main'.

C:\Users\Bernard\Documents\Gym\git>git remote
origin

C:\Users\Bernard\Documents\Gym\git>git remote add git-copy https://github.com/niyobern/Gym-Git-Exercise-Solution-2.git

C:\Users\Bernard\Documents\Gym\git>git add .

C:\Users\Bernard\Documents\Gym\git>git commit -m "pushing to both remotes"
[main a8ef400] pushing to both remotes
 1 file changed, 1 insertion(+)


C:\Users\Bernard\Documents\Gym\git>git push origin main && git push git-copy main 
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 2 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 307 bytes | 34.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/niyobern/Gym-Git-Exercise-Solution
   387b7b6..a8ef400  main -> main
Enumerating objects: 63, done.
Counting objects: 100% (63/63), done.
Delta compression using up to 2 threads
Compressing objects: 100% (56/56), done.
Writing objects: 100% (63/63), 18.37 KiB | 606.00 KiB/s, done.
Total 63 (delta 31), reused 15 (delta 4), pack-reused 0
remote: Resolving deltas: 100% (31/31), done.
To https://github.com/niyobern/Gym-Git-Exercise-Solution-2.git
 * [new branch]      main -> main

C:\Users\Bernard\Documents\Gym\git>

```

### Exercise 2

```bash

C:\Users\Bernard\Documents\git>git checkout -b ft/footer 
Switched to a new branch 'ft/footer'

C:\Users\Bernard\Documents\git>git add .

C:\Users\Bernard\Documents\git>git commit -m "changes for bundle 4 execise 2"
[ft/footer e1c7942] changes for bundle 4 execise 2
 1 file changed, 1 insertion(+), 1 deletion(-)    

C:\Users\Bernard\Documents\git>git add .

C:\Users\Bernard\Documents\git>git commit -m "other changes"
[ft/footer f0e66e8] other changes
 1 file changed, 3 insertions(+), 1 deletion(-)

C:\Users\Bernard\Documents\git>git push origin ft/footer
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 2 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 609 bytes | 76.00 KiB/s, done.
Total 6 (delta 4), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (4/4), completed with 2 local objects.
remote: 
remote: Create a pull request for 'ft/footer' on GitHub by visiting:
remote:      https://github.com/niyobern/Gym-Git-Exercise-Solution/pull/new/ft/footer
remote:
To https://github.com/niyobern/Gym-Git-Exercise-Solution
 * [new branch]      ft/footer -> ft/footer

C:\Users\Bernard\Documents\git>git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

C:\Users\Bernard\Documents\git>git branch ft/squashing


C:\Users\Bernard\Documents\git>git checkout ft/squashing
Switched to branch 'ft/squashing'

C:\Users\Bernard\Documents\git>git merge --squash ft/footer
Updating c8eaff4..f0e66e8
Fast-forward
Squash commit -- not updating HEAD
 home.html | 4 +++-
 1 file changed, 3 insertions(+), 1 deletion(-)

C:\Users\Bernard\Documents\git>git add .                               

C:\Users\Bernard\Documents\git>git commit -m "footer changes squashing"
[ft/squashing b07c882] footer changes squashing
 1 file changed, 3 insertions(+), 1 deletion(-)

C:\Users\Bernard\Documents\git>git push origin ft/squashing
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 2 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 344 bytes | 49.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
remote: 
remote: Create a pull request for 'ft/squashing' on GitHub by visiting:
remote:      https://github.com/niyobern/Gym-Git-Exercise-Solution/pull/new/ft/squashing
remote:
To https://github.com/niyobern/Gym-Git-Exercise-Solution
 * [new branch]      ft/squashing -> ft/squashing
C:\Users\Bernard\Documents\git>

```

## Bundle 5

### Exercise 1

Link: [https://niyobern.github.io/Gym-Git-Exercise-Solution/](https://niyobern.github.io/Gym-Git-Exercise-Solution/)

### Exercise 2


``` bash
C:\Users\Bernard\Documents\Gym>git clone https://github.com/niyobern/git-cafe-exercise.git
Cloning into 'git-cafe-exercise'...
remote: Enumerating objects: 107, done.
remote: Counting objects: 100% (7/7), done.
remote: Compressing objects: 100% (3/3), done.
Receiving objects: 100% (107/107), 1.95 MiB | 920.00 KiB/s, done.eceiving objects:  65% (70/107), 1.33 MiB | 808.00 KiB/s

Resolving deltas: 100% (5/5), done.
Updating files: 100% (106/106), done.

C:\Users\Bernard\Documents\Gym>cd git-cafe-exercise

C:\Users\Bernard\Documents\Gym\git-cafe-exercise>
C:\Users\Bernard\Documents\Gym\git-cafe-exercise>git add .

C:\Users\Bernard\Documents\Gym\git-cafe-exercise>git commit -m "changed index.htm"
[main 3b1abc2] changed index.htm
 1 file changed, 1 insertion(+), 1 deletion(-)

C:\Users\Bernard\Documents\Gym\git-cafe-exercise>git push origin main
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 2 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 316 bytes | 45.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/niyobern/git-cafe-exercise.git
   d1d3f9c..3b1abc2  main -> main

C:\Users\Bernard\Documents\Gym\git-cafe-exercise>

```
