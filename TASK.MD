# TASK 1

### 1-6

> arsen@ars-mi MINGW64 /c/Users/arsen/Desktop/git-task
> $ git init

> arsen@ars-mi MINGW64 /c/Users/arsen/Desktop/git-task (master)
> $ git branch -M main

> arsen@ars-mi MINGW64 /c/Users/arsen/Desktop/git-task (main)
> $ git remote add origin https://github.com/ars-shi/git-task.git

> arsen@ars-mi MINGW64 /c/Users/arsen/Desktop/git-task (master)

> $ vim TASK.MD

### 7-8

> arsen@ars-mi MINGW64 /c/Users/arsen/Desktop/git-task (main)
> $ git add .

> arsen@ars-mi MINGW64 /c/Users/arsen/Desktop/git-task (main)
> $ git commit -m "task 1 : 1-6"
``` 
[main (root-commit) 491a4a2] task 1 : 1-6
1 file changed, 17 insertions(+)
create mode 100644 TASK.MD 
```

> arsen@ars-mi MINGW64 /c/Users/arsen/Desktop/git-task (main)
> $ git push --set-upstream origin main
```
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 373 bytes | 373.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/ars-shi/git-task.git
 * [new branch]      main -> main
Branch 'main' set up to track remote branch 'main' from 'origin'.
```

 ### 9-12

> arsen@ars-mi MINGW64 /c/Users/arsen/Desktop/git-task (main)
> $ git diff
```
diff --git a/TASK.MD b/TASK.MD
index 63ee1cd..63be144 100644
--- a/TASK.MD
+++ b/TASK.MD
@@ -12,6 +12,17 @@
 > $ git remote add origin https://github.com/ars-shi/git-task.git

 > arsen@ars-mi MINGW64 /c/Users/arsen/Desktop/git-task (master)
+
 > $ vim TASK.MD

+### 7-8
+
+> arsen@ars-mi MINGW64 /c/Users/arsen/Desktop/git-task (main)
+> $ git add .
+
+> arsen@ars-mi MINGW64 /c/Users/arsen/Desktop/git-task (main)
+> $ git commit -m "task 1 : 1-6"
+``` [main (root-commit) 491a4a2] task 1 : 1-6
+ 1 file changed, 17 insertions(+)
+ create mode 100644 TASK.MD ```
```

> arsen@ars-mi MINGW64 /c/Users/arsen/Desktop/git-task (main)
> $ git status
```
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   TASK.MD

no changes added to commit (use "git add" and/or "git commit -a")
```

> arsen@ars-mi MINGW64 /c/Users/arsen/Desktop/git-task (main)
> $ git add .

> arsen@ars-mi MINGW64 /c/Users/arsen/Desktop/git-task (main)
> $ git commit -m "task 1: 11 (check status)"
```
[main a407e2b] task 1: 11 (check status)
 1 file changed, 61 insertions(+), 3 deletions(-)
```

> arsen@ars-mi MINGW64 /c/Users/arsen/Desktop/git-task (main)
> $ git status
```
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean
```

> arsen@ars-mi MINGW64 /c/Users/arsen/Desktop/git-task (main)
> $ git push
```
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 984 bytes | 984.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/ars-shi/git-task.git
   372ab29..a407e2b  main -> main
```

# Task 2

**[Task 2:6] "Задание выполнено успешно!:)"**



> arsen@ars-mi MINGW64 /c/Users/arsen/Desktop/git-task (main)
> $ git merge develop
```
Auto-merging TASK.MD
CONFLICT (content): Merge conflict in TASK.MD
Automatic merge failed; fix conflicts and then commit the result.
```

> arsen@ars-mi MINGW64 /c/Users/arsen/Desktop/git-task (main|MERGING)
> $ git status
```
On branch main
Your branch is up to date with 'origin/main'.

You have unmerged paths.
  (fix conflicts and run "git commit")
  (use "git merge --abort" to abort the merge)

Unmerged paths:
  (use "git add <file>..." to mark resolution)
        both modified:   TASK.MD

no changes added to commit (use "git add" and/or "git commit -a")
```

> arsen@ars-mi MINGW64 /c/Users/arsen/Desktop/git-task (main|MERGING)
> $ git mergetool
```
This message is displayed because 'merge.tool' is not configured.
See 'git mergetool --tool-help' or 'git help config' for more details.
'git mergetool' will now attempt to use one of the following tools:
opendiff kdiff3 tkdiff xxdiff meld tortoisemerge gvimdiff diffuse diffmerge ecmerge p4merge araxis bc codecompare smerge emerge vimdiff nvimdiff
Merging:
TASK.MD

Normal merge conflict for 'TASK.MD':
  {local}: modified file
  {remote}: modified file
Hit return to start merge resolution tool (vimdiff):
4 files to edit
```

>> arsen@ars-mi MINGW64 /c/Users/arsen/Desktop/git-task (main|MERGING)
>> $ git status
```
On branch main
Your branch is up to date with 'origin/main'.

All conflicts fixed but you are still merging.
  (use "git commit" to conclude merge)

Changes to be committed:
        modified:   TASK.MD

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        TASK.MD.orig
```

> arsen@ars-mi MINGW64 /c/Users/arsen/Desktop/git-task (main|MERGING)
> $ git commit -m "Task 2 : 6 (merge)"
```
[main c98af2e] Task 2 : 6 (merge)
```

> arsen@ars-mi MINGW64 /c/Users/arsen/Desktop/git-task (main)
> $ git push
```
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 304 bytes | 304.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/ars-shi/git-task.git
   65b6c43..c98af2e  main -> main
```

> arsen@ars-mi MINGW64 /c/Users/arsen/Desktop/git-task (main)
> $ git merge develop
```
Already up to date.
```
