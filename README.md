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