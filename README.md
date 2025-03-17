# push-branch-to-server



$ git branch -c developer0101

priya@MSI MINGW64 /d/gitLearnings/repositories/push-branch-to-server (main)
$ git branch --list
  developer0101
* main

priya@MSI MINGW64 /d/gitLearnings/repositories/push-branch-to-server (main)
$ git checkout developer0101
Switched to branch 'developer0101'
Your branch is up to date with 'origin/main'.

priya@MSI MINGW64 /d/gitLearnings/repositories/push-branch-to-server (developer0101)
$ git status
On branch developer0101
Your branch is up to date with 'origin/main'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        index01.html

nothing added to commit but untracked files present (use "git add" to track)

priya@MSI MINGW64 /d/gitLearnings/repositories/push-branch-to-server (developer0101)
$ git add .

priya@MSI MINGW64 /d/gitLearnings/repositories/push-branch-to-server (developer0101)
$ git commit -m "creating a static website"
[developer0101 8925d65] creating a static website
 1 file changed, 13 insertions(+)
 create mode 100644 index01.html

priya@MSI MINGW64 /d/gitLearnings/repositories/push-branch-to-server (developer0101)
$ git status
On branch developer0101
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   index01.html

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        about.html
        contact.html

no changes added to commit (use "git add" and/or "git commit -a")

priya@MSI MINGW64 /d/gitLearnings/repositories/push-branch-to-server (developer0101)
$ git add .

priya@MSI MINGW64 /d/gitLearnings/repositories/push-branch-to-server (developer0101)
$ git commit -m "modifications"
[developer0101 019754d] modifications
 3 files changed, 27 insertions(+), 1 deletion(-)
 create mode 100644 about.html
 create mode 100644 contact.html

priya@MSI MINGW64 /d/gitLearnings/repositories/push-branch-to-server (developer0101)
$ git swtich main
git: 'swtich' is not a git command. See 'git --help'.

The most similar command is
        switch

priya@MSI MINGW64 /d/gitLearnings/repositories/push-branch-to-server (developer0101)
$ git switch main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

priya@MSI MINGW64 /d/gitLearnings/repositories/push-branch-to-server (main)
$ git switch developer0101
Switched to branch 'developer0101'
Your branch is ahead of 'origin/main' by 2 commits.
  (use "git push" to publish your local commits)

priya@MSI MINGW64 /d/gitLearnings/repositories/push-branch-to-server (developer0101)
$ git push origin HEAD:developer0101
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 8 threads
Compressing objects: 100% (7/7), done.
Writing objects: 100% (7/7), 929 bytes | 929.00 KiB/s, done.
Total 7 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), done.
remote:
remote: Create a pull request for 'developer0101' on GitHub by visiting:
remote:      https://github.com/priya82573/push-branch-to-server/pull/new/developer0101
remote:
To https://github.com/priya82573/push-branch-to-server.git
 * [new branch]      HEAD -> developer0101

priya@MSI MINGW64 /d/gitLearnings/repositories/push-branch-to-server (developer0101)
$
