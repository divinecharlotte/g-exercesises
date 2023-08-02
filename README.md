# g-exercesises

### BUNDLE1

## EXERCESISE1

```

admin-MacBook-Pro:~ $ cd Desktop/
admin-MacBook-Pro:Desktop $ cd gym/
admin-MacBook-Pro:gym $ git clone https://github.com/divinecharlotte/g-exercesises.git
Cloning into 'g-exercesises'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (3/3), done.
admin-MacBook-Pro:gym $ cd g-exercesises/
admin-MacBook-Pro:g-exercesises $ code .
admin-MacBook-Pro:g-exercesises $ git add .
admin-MacBook-Pro:g-exercesises $ git commit -m "Bundle1 exercesise1"
[main 5c9a1c9] Bundle1 exercesise1
 1 file changed, 11 insertions(+)
 create mode 100644 index.html
admin-MacBook-Pro:g-exercesises $ git checkout -b dev
Switched to a new branch 'dev'
admin-MacBook-Pro:g-exercesises $ git checkout -b test
Switched to a new branch 'test'
admin-MacBook-Pro:g-exercesises $ git checkout dev
Switched to branch 'dev'
admin-MacBook-Pro:g-exercesises $ git branch -d test
Deleted branch test (was 5c9a1c9).
admin-MacBook-Pro:g-exercesises $
```

### EXERCESISE2

```
admin-MacBook-Pro:g-exercesises $ git stash list
stash@{0}: On dev: stash team.html
stash@{1}: On dev: stash about.html
stash@{2}: On dev: stash home.html
admin-MacBook-Pro:g-exercesises $ git stash pop stash@{X}
stash@{X} is not a valid reference
admin-MacBook-Pro:g-exercesises $ git stash pop stash@{2}
Already up to date!
On branch dev
Untracked files:
  (use "git add <file>..." to include in what will be committed)

        home.html

nothing added to commit but untracked files present (use "git add" to track)
Dropped stash@{2} (44272dc236832190701eb24c48b7ad6a64579f7d)
admin-MacBook-Pro:g-exercesises $ git add .
admin-MacBook-Pro:g-exercesises $ git commit -m "bundle1 exercesise2"
[dev 66edfd6] bundle1 exercesise2
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 home.html
admin-MacBook-Pro:g-exercesises $ git push origin dev
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 313 bytes | 313.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0)
To https://github.com/divinecharlotte/g-exercesises.git
   0114d68..66edfd6  dev -> dev
admin-MacBook-Pro:g-exercesises $ git stash pop stash@{0}
Already up to date!
On branch dev
Untracked files:
  (use "git add <file>..." to include in what will be committed)

        team.html

nothing added to commit but untracked files present (use "git add" to track)
Dropped stash@{0} (bdbf0abe2037ba99466530d7025997c01088f1e2)
admin-MacBook-Pro:g-exercesises $ git log --oneline
66edfd6 (HEAD -> dev, origin/dev) bundle1 exercesise2
0114d68 bundle1 exercesise1
5c9a1c9 (main) Bundle1 exercesise1
ed3be8e (origin/main, origin/HEAD) Initial commit
admin-MacBook-Pro:g-exercesises $ git reset --hard 66edfd6
HEAD is now at 66edfd6 bundle1 exercesise2
admin-MacBook-Pro:g-exercesises $
```
