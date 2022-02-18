# git_katas_repo

2nd katata terminal code : 
smrithi@Smrithis-MacBook-Air git_katas_repo %  echo 2 > file.txt
smrithi@Smrithis-MacBook-Air git_katas_repo % git diff
smrithi@Smrithis-MacBook-Air git_katas_repo % git diff --staged
smrithi@Smrithis-MacBook-Air git_katas_repo % git add file.txt
smrithi@Smrithis-MacBook-Air git_katas_repo % git diff
smrithi@Smrithis-MacBook-Air git_katas_repo % git diff --staged
diff --git a/file.txt b/file.txt
new file mode 100644
index 0000000..0cfbf08
--- /dev/null
+++ b/file.txt
@@ -0,0 +1 @@
+2
smrithi@Smrithis-MacBook-Air git_katas_repo % echo New > file.txt
smrithi@Smrithis-MacBook-Air git_katas_repo % git diff
diff --git a/file.txt b/file.txt
index 0cfbf08..96716fb 100644
--- a/file.txt
+++ b/file.txt
@@ -1 +1 @@
-2
+New
smrithi@Smrithis-MacBook-Air git_katas_repo % git diff --staged
diff --git a/file.txt b/file.txt
new file mode 100644
index 0000000..0cfbf08
--- /dev/null
+++ b/file.txt
@@ -0,0 +1 @@
+2
smrithi@Smrithis-MacBook-Air git_katas_repo % git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   file.txt

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   file.txt

smrithi@Smrithis-MacBook-Air git_katas_repo % git restore --staged file.txt
smrithi@Smrithis-MacBook-Air git_katas_repo % git status
On branch main
Your branch is up to date with 'origin/main'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        file.txt

nothing added to commit but untracked files present (use "git add" to track)
smrithi@Smrithis-MacBook-Air git_katas_repo % git add file.txt
smrithi@Smrithis-MacBook-Air git_katas_repo % git commit -m "First commit"
[main 1931b8c] First commit
 1 file changed, 1 insertion(+)
 create mode 100644 file.txt
smrithi@Smrithis-MacBook-Air git_katas_repo % git log
commit 1931b8c4404e42792d50df2d056129f6928e4ff9 (HEAD -> main)
Author: Smrithi M Menon <smrithi.menon@zemosolabs.com>
Date:   Fri Feb 18 17:41:14 2022 +0530

    First commit

commit 6e0056c772cbbbfe3ebb48f6c6057c0c96092ed5 (origin/main, origin/HEAD)
Author: Smrithi M Menon <smrithi.menon@zemosolabs.com>
Date:   Fri Feb 18 15:00:30 2022 +0530

    final commit

commit 54be04c82e24ffc76f598b19c52ee75abd0f75c3
Author: Smrithi M Menon <smrithi.menon@zemosolabs.com>
Date:   Fri Feb 18 14:02:39 2022 +0530

    final addition

commit 8aa366897f1dd21378ce1c35a483ccd9b640111e
Author: Smrithi M Menon <smrithi.menon@zemosolabs.com>
Date:   Fri Feb 18 13:50:19 2022 +0530

    initial commit

commit 866db19e6fe06132b968e4a1e86f415843ff42a8
Author: Smrithi M Menon <smrithi.menon@zemosolabs.com>
Date:   Fri Feb 18 10:45:32 2022 +0530

    first commit
smrithi@Smrithis-MacBook-Air git_katas_repo % 
smrithi@Smrithis-MacBook-Air git_katas_repo % git log -n 2
commit 1931b8c4404e42792d50df2d056129f6928e4ff9 (HEAD -> main)
Author: Smrithi M Menon <smrithi.menon@zemosolabs.com>
Date:   Fri Feb 18 17:41:14 2022 +0530

    First commit

commit 6e0056c772cbbbfe3ebb48f6c6057c0c96092ed5 (origin/main, origin/HEAD)
Author: Smrithi M Menon <smrithi.menon@zemosolabs.com>
Date:   Fri Feb 18 15:00:30 2022 +0530

    final commit
smrithi@Smrithis-MacBook-Air git_katas_repo % echo Overwriting now > file.txt
smrithi@Smrithis-MacBook-Air git_katas_repo % git status
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   file.txt

no changes added to commit (use "git add" and/or "git commit -a")
smrithi@Smrithis-MacBook-Air git_katas_repo % git restore file.txt
smrithi@Smrithis-MacBook-Air git_katas_repo % git status
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean
smrithi@Smrithis-MacBook-Air git_katas_repo % 







3rd katata terminal code : 
smrithi@Smrithis-MacBook-Air git_katas_repo % git branch
* main
smrithi@Smrithis-MacBook-Air git_katas_repo % git branch mybranch
smrithi@Smrithis-MacBook-Air git_katas_repo % git branch
* main
  mybranch
smrithi@Smrithis-MacBook-Air git_katas_repo % git switch mybranch
Switched to branch 'mybranch'
smrithi@Smrithis-MacBook-Air git_katas_repo % git status
On branch mybranch
nothing to commit, working tree clean
smrithi@Smrithis-MacBook-Air git_katas_repo % git switch main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
smrithi@Smrithis-MacBook-Air git_katas_repo % git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean
smrithi@Smrithis-MacBook-Air git_katas_repo % git switch mybranch
Switched to branch 'mybranch'
smrithi@Smrithis-MacBook-Air git_katas_repo % git add file1.txt
smrithi@Smrithis-MacBook-Air git_katas_repo % git commit -m "committing Smrithi"
[mybranch 0da3129] committing Smrithi
 1 file changed, 1 insertion(+)
 create mode 100644 file1.txt
smrithi@Smrithis-MacBook-Air git_katas_repo % git log --online --graph
fatal: unrecognized argument: --online
smrithi@Smrithis-MacBook-Air git_katas_repo % git log --oneline --graph
* 0da3129 (HEAD -> mybranch) committing Smrithi
* 830480e (origin/main, origin/HEAD, main) commit for 2nd katata
* 1931b8c First commit
* 6e0056c final commit
* 54be04c final addition
* 8aa3668 initial commit
* 866db19 first commit
smrithi@Smrithis-MacBook-Air git_katas_repo % git switch main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
smrithi@Smrithis-MacBook-Air git_katas_repo % git log --oneline --graph
* 830480e (HEAD -> main, origin/main, origin/HEAD) commit for 2nd katata
* 1931b8c First commit
* 6e0056c final commit
* 54be04c final addition
* 8aa3668 initial commit
* 866db19 first commit
smrithi@Smrithis-MacBook-Air git_katas_repo % git add file2.txt             
smrithi@Smrithis-MacBook-Air git_katas_repo % git commit -m "committing main branch file"
[main 403c102] committing main branch file
 1 file changed, 1 insertion(+)
 create mode 100644 file2.txt
smrithi@Smrithis-MacBook-Air git_katas_repo % git log --oneline --graph all
fatal: ambiguous argument 'all': unknown revision or path not in the working tree.
Use '--' to separate paths from revisions, like this:
'git <command> [<revision>...] -- [<file>...]'
smrithi@Smrithis-MacBook-Air git_katas_repo % git log --oneline --graph
* 403c102 (HEAD -> main) committing main branch file
* 830480e (origin/main, origin/HEAD) commit for 2nd katata
* 1931b8c First commit
* 6e0056c final commit
* 54be04c final addition
* 8aa3668 initial commit
* 866db19 first commit
smrithi@Smrithis-MacBook-Air git_katas_repo % git log --oneline --graph --all
* 403c102 (HEAD -> main) committing main branch file
| * 0da3129 (mybranch) committing Smrithi
|/  
* 830480e (origin/main, origin/HEAD) commit for 2nd katata
* 1931b8c First commit
* 6e0056c final commit
* 54be04c final addition
* 8aa3668 initial commit
* 866db19 first commit
smrithi@Smrithis-MacBook-Air git_katas_repo % git switch mybranch
Switched to branch 'mybranch'
smrithi@Smrithis-MacBook-Air git_katas_repo % git diff mybranch main
diff --git a/file1.txt b/file1.txt
deleted file mode 100644
index e5f51b3..0000000
--- a/file1.txt
+++ /dev/null
@@ -1 +0,0 @@
-Smrithi
\ No newline at end of file
diff --git a/file2.txt b/file2.txt
new file mode 100644
index 0000000..872be83
--- /dev/null
+++ b/file2.txt
@@ -0,0 +1 @@
+Main branch file
\ No newline at end of file
smrithi@Smrithis-MacBook-Air git_katas_repo % 