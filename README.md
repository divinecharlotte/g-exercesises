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

## BUNDLE2

### EXERCESISE1

```
admin-MacBook-Pro:g-exercesises $ git checkout -b ft/bundle-2
Switched to a new branch 'ft/bundle-2'
admin-MacBook-Pro:g-exercesises $ git add .
admin-MacBook-Pro:g-exercesises $ git add .
admin-MacBook-Pro:g-exercesises $ git commit -m "bundle2 exercesise1"
[ft/bundle-2 48a1791] bundle2 exercesise1
 1 file changed, 11 insertions(+)
 create mode 100644 services.html
admin-MacBook-Pro:g-exercesises $ git push origin ft/bundle-2
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 423 bytes | 423.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote:      https://github.com/divinecharlotte/g-exercesises/pull/new/ft/bundle-2
remote:
To https://github.com/divinecharlotte/g-exercesises.git
 * [new branch]      ft/bundle-2 -> ft/bundle-2
admin-MacBook-Pro:g-exercesises $
```

### EXERCESISE2

````
admin-MacBook-Pro:g-exercesises $ git checkout main
Switched to branch 'main'
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)
admin-MacBook-Pro:g-exercesises $ git checkout -b ft/service-redesign
Switched to a new branch 'ft/service-redesign'
admin-MacBook-Pro:g-exercesises $ git add .
admin-MacBook-Pro:g-exercesises $ git commit -m "bundle2 exercesise2"
[ft/service-redesign f746b2b] bundle2 exercesise2
 1 file changed, 11 insertions(+)
 create mode 100644 service.html
admin-MacBook-Pro:g-exercesises $ git push
admin-MacBook-Pro:g-exercesises $ git push origin ft/service-redesign
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 468 bytes | 468.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0)
remote:
remote: Create a pull request for 'ft/service-redesign' on GitHub by visiting:
remote:      https://github.com/divinecharlotte/g-exercesises/pull/new/ft/service-redesign
remote:
To https://github.com/divinecharlotte/g-exercesises.git
 * [new branch]      ft/service-redesign -> ft/service-redesign
admin-MacBook-Pro:g-exercesises $ git checkout main
Switched to branch 'main'
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)
admin-MacBook-Pro:g-exercesises $ git add .
admin-MacBook-Pro:g-exercesises $ git commit -m "bundle2 exercesise2 on main"
[main 9c9271b] bundle2 exercesise2 on main
 1 file changed, 11 insertions(+)
 create mode 100644 service.html
admin-MacBook-Pro:g-exercesises $ git pull
remote: Enumerating objects: 1, done.
remote: Counting objects: 100% (1/1), done.
remote: Total 1 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (1/1), done.
From https://github.com/divinecharlotte/g-exercesises
   ed3be8e..4eac444  main       -> origin/main
Merge made by the 'recursive' strategy.
 README.md | 87 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-
 home.html |  0
 team.html |  0
 3 files changed, 86 insertions(+), 1 deletion(-)
 create mode 100644 home.html
 create mode 100644 team.html
admin-MacBook-Pro:g-exercesises $ git push
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 4 threads
Compressing objects: 100% (5/5), done.
Writing objects: 100% (5/5), 770 bytes | 770.00 KiB/s, done.
Total 5 (delta 1), reused 0 (delta 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/divinecharlotte/g-exercesises.git
   4eac444..06b7aea  main -> main
admin-MacBook-Pro:g-exercesises $ ft/service-redesign
bash: ft/service-redesign: No such file or directory
admin-MacBook-Pro:g-exercesises $ git checkout ft/service-redesign
Switched to branch 'ft/service-redesign'
admin-MacBook-Pro:g-exercesises $ git diff main
diff --git a/README.md b/README.md
index 12ccf78..640de47 100644
--- a/README.md
+++ b/README.md
@@ -1,86 +1 @@
-# g-exercesises
-
-### BUNDLE1
-
-## EXERCESISE1
-
-```
-
-admin-MacBook-Pro:~ $ cd Desktop/
-admin-MacBook-Pro:Desktop $ cd gym/
-admin-MacBook-Pro:gym $ git clone https://github.com/divinecharlotte/g-exercesises.git
-Cloning into 'g-exercesises'...
-remote: Enumerating objects: 3, done.
-remote: Counting objects: 100% (3/3), done.
-remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
-Unpacking objects: 100% (3/3), done.
-admin-MacBook-Pro:gym $ cd g-exercesises/
-admin-MacBook-Pro:g-exercesises $ code .
-admin-MacBook-Pro:g-exercesises $ git add .
-admin-MacBook-Pro:g-exercesises $ git commit -m "Bundle1 exercesise1"
-[main 5c9a1c9] Bundle1 exercesise1
- 1 file changed, 11 insertions(+)
- create mode 100644 index.html
-admin-MacBook-Pro:g-exercesises $ git checkout -b dev
-Switched to a new branch 'dev'
-admin-MacBook-Pro:g-exercesises $ git checkout -b test
-Switched to a new branch 'test'
-admin-MacBook-Pro:g-exercesises $ git checkout dev
-Switched to branch 'dev'
-admin-MacBook-Pro:g-exercesises $ git branch -d test
-Deleted branch test (was 5c9a1c9).
-admin-MacBook-Pro:g-exercesises $
-```
-
-### EXERCESISE2
-
-```
-admin-MacBook-Pro:g-exercesises $ git stash list
-stash@{0}: On dev: stash team.html
-stash@{1}: On dev: stash about.html
-stash@{2}: On dev: stash home.html
-admin-MacBook-Pro:g-exercesises $ git stash pop stash@{X}
-stash@{X} is not a valid reference
-admin-MacBook-Pro:g-exercesises $ git stash pop stash@{2}
-Already up to date!
-On branch dev
-Untracked files:
-  (use "git add <file>..." to include in what will be committed)
-
-        home.html
-
-nothing added to commit but untracked files present (use "git add" to track)
-Dropped stash@{2} (44272dc236832190701eb24c48b7ad6a64579f7d)
-admin-MacBook-Pro:g-exercesises $ git add .
-admin-MacBook-Pro:g-exercesises $ git commit -m "bundle1 exercesise2"
-[dev 66edfd6] bundle1 exercesise2
- 1 file changed, 0 insertions(+), 0 deletions(-)
- create mode 100644 home.html
-admin-MacBook-Pro:g-exercesises $ git push origin dev
-Enumerating objects: 4, done.
-Counting objects: 100% (4/4), done.
-Delta compression using up to 4 threads
-Compressing objects: 100% (2/2), done.
-Writing objects: 100% (3/3), 313 bytes | 313.00 KiB/s, done.
-Total 3 (delta 0), reused 0 (delta 0)
-To https://github.com/divinecharlotte/g-exercesises.git
-   0114d68..66edfd6  dev -> dev
-admin-MacBook-Pro:g-exercesises $ git stash pop stash@{0}
-Already up to date!
-On branch dev
-Untracked files:
-  (use "git add <file>..." to include in what will be committed)
-
-        team.html
-
-nothing added to commit but untracked files present (use "git add" to track)
-Dropped stash@{0} (bdbf0abe2037ba99466530d7025997c01088f1e2)
-admin-MacBook-Pro:g-exercesises $ git log --oneline
-66edfd6 (HEAD -> dev, origin/dev) bundle1 exercesise2
-0114d68 bundle1 exercesise1
:
Your branch is up to date with 'origin/main'.
admin-MacBook-Pro:g-exercesises $ git merge ft/service-redesign
Auto-merging service.html
CONFLICT (add/add): Merge conflict in service.html
Automatic merge failed; fix conflicts and then commit the result.
admin-MacBook-Pro:g-exercesises $ git add .
admin-MacBook-Pro:g-exercesises $ git checkout git merge ft/service-redesign
error: pathspec 'git' did not match any file(s) known to git
error: pathspec 'merge' did not match any file(s) known to git
error: pathspec 'ft/service-redesign' did not match any file(s) known to git
admin-MacBook-Pro:g-exercesises $ git add .
admin-MacBook-Pro:g-exercesises $ git commit -m "bubsle 2 ex
ercesise2 "
[ft/bundle-2 970f0fd] bubsle 2 exercesise2
 1 file changed, 197 insertions(+)
admin-MacBook-Pro:g-exercesises $ git push origin ft/bundle-2
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 4 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 2.69 KiB | 2.69 MiB/s, done.
Total 6 (delta 3), reused 0 (delta 0)
remote: Resolving deltas: 100% (3/3), completed with 1 local object.
To https://github.com/divinecharlotte/g-exercesises.git
   48a1791..970f0fd  ft/bundle-2 -> ft/bundle-2
admin-MacBook-Pro:g-exercesises $
````

## BUNDLE3

### EXERCESISE1

```
bash: no job control in this shell
admin-MacBook-Pro:g-exercesises $ git checkout -b ft/team-page
Switched to a new branch 'ft/team-page'
admin-MacBook-Pro:g-exercesises $ git add .
admin-MacBook-Pro:g-exercesises $ git commit -m "bundle3 exercesise1"
[ft/team-page c67cbf3] bundle3 exercesise1
 1 file changed, 11 insertions(+)
admin-MacBook-Pro:g-exercesises $ git push origin ft/team-page
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 405 bytes | 405.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/team-page' on GitHub by visiting:
remote:      https://github.com/divinecharlotte/g-exercesises/pull/new/ft/team-page
remote:
To https://github.com/divinecharlotte/g-exercesises.git
 * [new branch]      ft/team-page -> ft/team-page
admin-MacBook-Pro:g-exercesises $ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
admin-MacBook-Pro:g-exercesises $ git checkout -b ft/contact-page
Switched to a new branch 'ft/contact-page'
admin-MacBook-Pro:g-exercesises $ git checkout ft/team-page
Switched to branch 'ft/team-page'
admin-MacBook-Pro:g-exercesises $ git log --oneline
c67cbf3 (HEAD -> ft/team-page, origin/ft/team-page) bundle3 exercesise1
df380d8 (origin/ft/bundle-2, ft/bundle-2) bubsle 2 exercesise2
970f0fd bubsle 2 exercesise2
e288322 bundle2 exercesise1
48a1791 bundle2 exercesise1
3f9e538 (origin/dev, dev) bundle1 exercesise2
66edfd6 bundle1 exercesise2
0114d68 bundle1 exercesise1
5c9a1c9 Bundle1 exercesise1
ed3be8e Initial commit
admin-MacBook-Pro:g-exercesises $ git checkout ft/contact-page
Switched to branch 'ft/contact-page'
admin-MacBook-Pro:g-exercesises $  git cherry-pick c67cbf3
[ft/contact-page 8bb1610] bundle3 exercesise1
 Date: Thu Aug 3 10:24:28 2023 +0200
 1 file changed, 11 insertions(+)
admin-MacBook-Pro:g-exercesises $ git add .
admin-MacBook-Pro:g-exercesises $ git commit -m "bundle3 exercesise1"
[ft/contact-page 7bf637d] bundle3 exercesise1
 1 file changed, 11 insertions(+)
 create mode 100644 contact.html
admin-MacBook-Pro:g-exercesises $ git push origin ft/contact-page
Enumerating objects: 19, done.
Counting objects: 100% (18/18), done.
Delta compression using up to 4 threads
Compressing objects: 100% (13/13), done.
Writing objects: 100% (13/13), 2.38 KiB | 2.38 MiB/s, done.
Total 13 (delta 5), reused 0 (delta 0)
remote: Resolving deltas: 100% (5/5), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/contact-page' on GitHub by visiting:
remote:      https://github.com/divinecharlotte/g-exercesises/pull/new/ft/contact-page
remote:
To https://github.com/divinecharlotte/g-exercesises.git
 * [new branch]      ft/contact-page -> ft/contact-page
admin-MacBook-Pro:g-exercesises $ git checkout -b ft/faq-page
Switched to a new branch 'ft/faq-page'
admin-MacBook-Pro:g-exercesises $ git add .
admin-MacBook-Pro:g-exercesises $ git commit -m "bundle3 exercesise1"
[ft/faq-page 4d91261] bundle3 exercesise1
 1 file changed, 11 insertions(+)
 create mode 100644 faq.html
admin-MacBook-Pro:g-exercesises $ git push origin ft/faq-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 417 bytes | 417.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/faq-page' on GitHub by visiting:
remote:      https://github.com/divinecharlotte/g-exercesises/pull/new/ft/faq-page
remote:
To https://github.com/divinecharlotte/g-exercesises.git
 * [new branch]      ft/faq-page -> ft/faq-page
git checkout ft/team-page
Switched to branch 'ft/team-page'
admin-MacBook-Pro:g-exercesises $ git log
commit c67cbf31b881bef04f0f3aea62a8103620c4d1b4 (HEAD -> ft/team-page, origin/ft/team-page)
Author: charlotte divine <divinemaina@gmail.com>
Date:   Thu Aug 3 10:24:28 2023 +0200

    bundle3 exercesise1

commit df380d8b43de6ac074b51559a62eef52e5c51bbf (origin/ft/bundle-2, ft/bundle-2)
Author: charlotte divine <divinemaina@gmail.com>
Date:   Wed Aug 2 12:26:41 2023 +0200

    bubsle 2 exercesise2

commit 970f0fdef8991889312679f0647efc2cc4cd7626
Author: charlotte divine <divinemaina@gmail.com>
Date:   Wed Aug 2 12:25:17 2023 +0200
:
admin-MacBook-Pro:g-exercesises $  git revert c67cbf31b881be
f04f0f3aea62a8103620c4d1b4
[ft/team-page 0cfe73f] Revert "bundle3 exercesise1"
 1 file changed, 11 deletions(-)
admin-MacBook-Pro:g-exercesises $ git add .
admin-MacBook-Pro:g-exercesises $ git commit -m "bundle3 exercesise1"
On branch ft/team-page
nothing to commit, working tree clean
admin-MacBook-Pro:g-exercesises $ git push origin ft/team-page
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 257 bytes | 257.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/divinecharlotte/g-exercesises.git
   c67cbf3..0cfe73f  ft/team-page -> ft/team-page
admin-MacBook-Pro:g-exercesises $
```

### EXERCISE2

```
admin-MacBook-Pro:g-exercesises $ git checkout ft/faq-page
Switched to branch 'ft/faq-page'
admin-MacBook-Pro:g-exercesises $ git checkout -b ft/home-page-redesign
Switched to a new branch 'ft/home-page-redesign'
admin-MacBook-Pro:g-exercesises $ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
admin-MacBook-Pro:g-exercesises $ git add .
admin-MacBook-Pro:g-exercesises $ git commit -m "bundle 3 exercesise2"
[main 4999a77] bundle 3 exercesise2
 1 file changed, 1 insertion(+), 1 deletion(-)
admin-MacBook-Pro:g-exercesises $ git push
Enumerating objects: 9, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 4 threads
Compressing objects: 100% (5/5), done.
Writing objects: 100% (5/5), 614 bytes | 614.00 KiB/s, done.
Total 5 (delta 3), reused 0 (delta 0)
remote: Resolving deltas: 100% (3/3), completed with 3 local objects.
To https://github.com/divinecharlotte/g-exercesises.git
   92f5d9a..df9801c  main -> main
admin-MacBook-Pro:g-exercesises $ git checkout ft/home-page-redesign
Switched to branch 'ft/home-page-redesign'
admin-MacBook-Pro:g-exercesises $ git rebase main
First, rewinding head to replay your work on top of it...
Applying: bundle3 exercesise1
Applying: bundle3 exercesise1
Applying: bundle3 exercesise1
admin-MacBook-Pro:g-exercesises $ git add .
admin-MacBook-Pro:g-exercesises $ git commit -m "bundle 3 exercesise2"
[ft/home-page-redesign 515fa4c] bundle 3 exercesise2
 1 file changed, 11 insertions(+)
admin-MacBook-Pro:g-exercesises $ git push origin ft/home-page-redesign
Enumerating objects: 15, done.
Counting objects: 100% (14/14), done.
Delta compression using up to 4 threads
Compressing objects: 100% (12/12), done.
Writing objects: 100% (12/12), 1.23 KiB | 1.23 MiB/s, done.
Total 12 (delta 6), reused 0 (delta 0)
remote: Resolving deltas: 100% (6/6), done.
remote:
remote: Create a pull request for 'ft/home-page-redesign' on GitHub by visiting:
remote:      https://github.com/divinecharlotte/g-exercesises/pull/new/ft/home-page-redesign
remote:
To https://github.com/divinecharlotte/g-exercesises.git
 * [new branch]      ft/home-page-redesign -> ft/home-page-redesign
admin-MacBook-Pro:g-exercesises $

```
