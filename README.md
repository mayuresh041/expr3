C:\Users\91987>cd rev1

C:\Users\91987\rev1>git checkout -b fb1
fatal: a branch named 'fb1' already exists

C:\Users\91987\rev1>git checkout fb1
Switched to branch 'fb1'

C:\Users\91987\rev1>rev1.txt

C:\Users\91987\rev1>git add .

C:\Users\91987\rev1>git stash save "stashing"
Saved working directory and index state On fb1: stashing

C:\Users\91987\rev1>git checkout -b tb1
Switched to a new branch 'tb1'

C:\Users\91987\rev1>git stash list
stash@{0}: On fb1: stashing

C:\Users\91987\rev1>git stash apply stash@{0}
On branch tb1
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   rev1.txt

no changes added to commit (use "git add" and/or "git commit -a")

C:\Users\91987\rev1>git add .

C:\Users\91987\rev1>git commit -m "second commit "
[tb1 6cd3c13] second commit
 1 file changed, 1 insertion(+)

C:\Users\91987\rev1>rev1.txt

C:\Users\91987\rev1>git checkout master
Switched to branch 'master'

C:\Users\91987\rev1>git merge tb1
Updating 119999e..6cd3c13
Fast-forward
 rev1.txt | 1 +
 1 file changed, 1 insertion(+)

C:\Users\91987\rev1>rev1.txt

C:\Users\91987\rev1># expr3
