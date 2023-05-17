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


### Exercises 2

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

C:\Users\bernard\documents\Gym\git>git branch ft/bundle-2

C:\Users\bernard\documents\Gym\git>

```