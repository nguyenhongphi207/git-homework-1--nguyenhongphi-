PartA:
1.nguyen-hong-phi@nguyen-hong-phi-HP-245-G8-Notebook-PC:~/git-homework-1/part1$ git add week2.md
nguyen-hong-phi@nguyen-hong-phi-HP-245-G8-Notebook-PC:~/git-homework-1/part1$ git commit -m createw2
[main b72e0d0] createw2
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 part1/week2.md

nguyen-hong-phi@nguyen-hong-phi-HP-245-G8-Notebook-PC:~/git-homework-1/part1$ git branch week2
nguyen-hong-phi@nguyen-hong-phi-HP-245-G8-Notebook-PC:~/git-homework-1/part1$ git switch week2
Switched to branch 'week2'

2.
nguyen-hong-phi@nguyen-hong-phi-HP-245-G8-Notebook-PC:~/git-homework-1/part1$ git add week2.md
nguyen-hong-phi@nguyen-hong-phi-HP-245-G8-Notebook-PC:~/git-homework-1/part1$ git commit -m working1
[week2 5ac5591] working1
 1 file changed, 1 insertion(+)

nguyen-hong-phi@nguyen-hong-phi-HP-245-G8-Notebook-PC:~/git-homework-1/part1$ git add week2.md
nguyen-hong-phi@nguyen-hong-phi-HP-245-G8-Notebook-PC:~/git-homework-1/part1$ git commit -m working2
[week2 6be3c40] working2
 1 file changed, 1 insertion(+)

3.nguyen-hong-phi@nguyen-hong-phi-HP-245-G8-Notebook-PC:~/git-homework-1/part1$ git add week2.md
nguyen-hong-phi@nguyen-hong-phi-HP-245-G8-Notebook-PC:~/git-homework-1/part1$ git commit -m insert
[week2 1285723] insert
 1 file changed, 2 insertions(+), 1 deletion(-)

nguyen-hong-phi@nguyen-hong-phi-HP-245-G8-Notebook-PC:~/git-homework-1/part1$ git switch main
Switched to branch 'main'
Your branch is ahead of 'origin/main' by 2 commits.
  (use "git push" to publish your local commits)

4.
nguyen-hong-phi@nguyen-hong-phi-HP-245-G8-Notebook-PC:~/git-homework-1/part1$ git switch -c week2b
Switched to a new branch 'week2b'

partB 

1.
nguyen-hong-phi@nguyen-hong-phi-HP-245-G8-Notebook-PC:~/git-homework-1/part1$ git merge week2
Merge made by the 'ort' strategy.
 part1/week2.md | 3 +++
 1 file changed, 3 insertions(+)

nguyen-hong-phi@nguyen-hong-phi-HP-245-G8-Notebook-PC:~/git-homework-1/part1$ git branch -d week2
Deleted branch week2 (was 1285723).
nguyen-hong-phi@nguyen-hong-phi-HP-245-G8-Notebook-PC:~/git-homework-1/part1$ git switch -c wip
Switched to a new branch 'wip'
nguyen-hong-phi@nguyen-hong-phi-HP-245-G8-Notebook-PC:~/git-homework-1/part1$ touch wip.txt
nguyen-hong-phi@nguyen-hong-phi-HP-245-G8-Notebook-PC:~/git-homework-1/part1$ git add wip.txt
nguyen-hong-phi@nguyen-hong-phi-HP-245-G8-Notebook-PC:~/git-homework-1/part1$ git commit -m "add wip.txt"
[wip 189659c] add wip.txt
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 part1/wip.txt

nguyen-hong-phi@nguyen-hong-phi-HP-245-G8-Notebook-PC:~/git-homework-1/part1$ git merge week2b
Updating 8d2665f..ab4798c
Fast-forward
 part1/week2.md        |  3 +++
 part1/week2_report.md | 33 +++++++++++++++++++++++++++++++++
 2 files changed, 36 insertions(+)
 create mode 100644 part1/week2_report.md

2.
nguyen-hong-phi@nguyen-hong-phi-HP-245-G8-Notebook-PC:~/git-homework-1/part1$ git branch --merged
* main
  week2b
nguyen-hong-phi@nguyen-hong-phi-HP-245-G8-Notebook-PC:~/git-homework-1/part1$ git branch --no-merged
  huyduong
  users
  wip

3.
nguyen-hong-phi@nguyen-hong-phi-HP-245-G8-Notebook-PC:~/git-homework-1/part1$ git branch -d week2b
Deleted branch week2b (was ab4798c).

4.
nguyen-hong-phi@nguyen-hong-phi-HP-245-G8-Notebook-PC:~/git-homework-1/part1$ git branch --move wip work-in-progress
nguyen-hong-phi@nguyen-hong-phi-HP-245-G8-Notebook-PC:~/git-homework-1/part1$ git push origin -u work-in-progress
Enumerating objects: 39, done.
Counting objects: 100% (39/39), done.
Delta compression using up to 8 threads
Compressing objects: 100% (33/33), done.
Writing objects: 100% (37/37), 3.46 KiB | 885.00 KiB/s, done.
Total 37 (delta 17), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (17/17), completed with 2 local objects.
remote: 
remote: Create a pull request for 'work-in-progress' on GitHub by visiting:
remote:      https://github.com/nguyenhongphi207/git-homework-1--nguyenhongphi-/pull/new/work-in-progress
remote: 
To https://github.com/nguyenhongphi207/git-homework-1--nguyenhongphi-.git
 * [new branch]      work-in-progress -> work-in-progress
branch 'work-in-progress' set up to track 'origin/work-in-progress'.
nguyen-hong-phi@nguyen-hong-phi-HP-245-G8-Notebook-PC:~/git-homework-1/part1$ git switch work-in-progress
Switched to branch 'work-in-progress'
Your branch is up to date with 'origin/work-in-progress'.

Part c
1.nguyen-hong-phi@nguyen-hong-phi-HP-245-G8-Notebook-PC:~/git-homework-1/part1$ git add wip.txt
nguyen-hong-phi@nguyen-hong-phi-HP-245-G8-Notebook-PC:~/git-homework-1/part1$ git commit -m "add text to wip"
[work-in-progress f20b449] add text to wip
 1 file changed, 1 insertion(+)

2.
nguyen-hong-phi@nguyen-hong-phi-HP-245-G8-Notebook-PC:~/git-homework-1/part1$ git branch -vv
  huyduong         f67360b [origin/huyduong] rename
  main             ab4798c [origin/main: ahead 8] Merge branch 'week2' into week2b
  users            823c52a [origin/users] fckhuyduong
* work-in-progress f20b449 [origin/work-in-progress: ahead 2] add text to wip


Part D.
1.
nguyen-hong-phi@nguyen-hong-phi-HP-245-G8-Notebook-PC:~/git-homework-1/part1$ git switch -c experiment
Switched to a new branch 'experiment'
nguyen-hong-phi@nguyen-hong-phi-HP-245-G8-Notebook-PC:~/git-homework-1/part1$ touch file1.txt
nguyen-hong-phi@nguyen-hong-phi-HP-245-G8-Notebook-PC:~/git-homework-1/part1$ git add file1.txt
nguyen-hong-phi@nguyen-hong-phi-HP-245-G8-Notebook-PC:~/git-homework-1/part1$ git commit -m "experiment commit 1"
[experiment d052cf2] experiment commit 1
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 part1/file1.txt
nguyen-hong-phi@nguyen-hong-phi-HP-245-G8-Notebook-PC:~/git-homework-1/part1$ touch file2.txt
nguyen-hong-phi@nguyen-hong-phi-HP-245-G8-Notebook-PC:~/git-homework-1/part1$ git add file2.txt
nguyen-hong-phi@nguyen-hong-phi-HP-245-G8-Notebook-PC:~/git-homework-1/part1$ git commit -m "experiment commit 2"
[experiment ad8c6fa] experiment commit 2
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 part1/file2.txt

2.
nguyen-hong-phi@nguyen-hong-phi-HP-245-G8-Notebook-PC:~/git-homework-1/part1$ git switch main
Switched to branch 'main'
Your branch is ahead of 'origin/main' by 8 commits.
  (use "git push" to publish your local commits)
nguyen-hong-phi@nguyen-hong-phi-HP-245-G8-Notebook-PC:~/git-homework-1/part1$ touch file3.txt
nguyen-hong-phi@nguyen-hong-phi-HP-245-G8-Notebook-PC:~/git-homework-1/part1$ git add file3.txt
nguyen-hong-phi@nguyen-hong-phi-HP-245-G8-Notebook-PC:~/git-homework-1/part1$ git commit -m "main commit"
[main 91af5ae] main commit
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 part1/file3.txt

3.
nguyen-hong-phi@nguyen-hong-phi-HP-245-G8-Notebook-PC:~/git-homework-1/part1$ git switch experiment
Switched to branch 'experiment'

nguyen-hong-phi@nguyen-hong-phi-HP-245-G8-Notebook-PC:~/git-homework-1/part1$ git rebase main
Current branch experiment is up to date.

4.rebase lấy các commit của experiment (2 commit ở bước 1), "gỡ" chúng ra, sau đó "gắn lại" (replay) từng commit đó lên trên đầu mới nhất của master (commit ở bước 2). Kết quả là lịch sử của experiment trở thành một đường thẳng nối tiếp sau master, thay vì bị phân nhánh — commit ID của các commit trên experiment sẽ thay đổi vì chúng được tạo lại (replay) trên nền mới.

5.
nguyen-hong-phi@nguyen-hong-phi-HP-245-G8-Notebook-PC:~/git-homework-1/part1$ git switch main
Switched to branch 'main'
Your branch is ahead of 'origin/main' by 9 commits.
  (use "git push" to publish your local commits)
nguyen-hong-phi@nguyen-hong-phi-HP-245-G8-Notebook-PC:~/git-homework-1/part1$ git merge experiment
Updating 91af5ae..8b97d68
Fast-forward
 part1/file1.txt | 0
 part1/file2.txt | 0
 2 files changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 part1/file1.txt
 create mode 100644 part1/file2.txt