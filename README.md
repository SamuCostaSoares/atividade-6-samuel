
samuc@LAPTOP-1UVA8F1I MINGW64 ~/Documents/atividade-6-samuel (master)
$ git branch -M "main"]

samuc@LAPTOP-1UVA8F1I MINGW64 ~/Documents/atividade-6-samuel (main])
$ git branch -M "main"

samuc@LAPTOP-1UVA8F1I MINGW64 ~/Documents/atividade-6-samuel (main)
$ git init
Initialized empty Git repository in C:/Users/samuc/Documents/atividade-6-samuel/.git/

samuc@LAPTOP-1UVA8F1I MINGW64 ~/Documents/atividade-6-samuel (master)
$ git branch -M "main"

samuc@LAPTOP-1UVA8F1I MINGW64 ~/Documents/atividade-6-samuel (main)
$ git add .

samuc@LAPTOP-1UVA8F1I MINGW64 ~/Documents/atividade-6-samuel (main)
$ git commit -m "primeiro commit"
[main (root-commit) 2397d80] primeiro commit
 3 files changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 README.md
 create mode 100644 arquivos1.js
 create mode 100644 arquivos2.js

samuc@LAPTOP-1UVA8F1I MINGW64 ~/Documents/atividade-6-samuel (main)
$ git tag -a v1.0 -m "versão de inicio"

samuc@LAPTOP-1UVA8F1I MINGW64 ~/Documents/atividade-6-samuel (main)
$ git tag
v1.0

samuc@LAPTOP-1UVA8F1I MINGW64 ~/Documents/atividade-6-samuel (main)
$ git add .

samuc@LAPTOP-1UVA8F1I MINGW64 ~/Documents/atividade-6-samuel (main)
$  git commit -m "segundo commit"
[main dd9a2a6] segundo commit
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 arquivos3.js

samuc@LAPTOP-1UVA8F1I MINGW64 ~/Documents/atividade-6-samuel (main)
$ git remote add origin https://github.com/Shimu192/atividade-6-samuel.git

samuc@LAPTOP-1UVA8F1I MINGW64 ~/Documents/atividade-6-samuel (main)
$ git push -u origin main --tags
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 2 threads
Compressing objects: 100% (5/5), done.
Writing objects: 100% (6/6), 535 bytes | 33.00 KiB/s, done.
Total 6 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), done.
To https://github.com/Shimu192/atividade-6-samuel.git
 * [new branch]      main -> main
 * [new tag]         v1.0 -> v1.0
Branch 'main' set up to track remote branch 'main' from 'origin'.

samuc@LAPTOP-1UVA8F1I MINGW64 ~/Documents/atividade-6-samuel (main)
$ git checkout "dev"
error: pathspec 'dev' did not match any file(s) known to git

samuc@LAPTOP-1UVA8F1I MINGW64 ~/Documents/atividade-6-samuel (main)
$ git checkout -b "dev"
Switched to a new branch 'dev'

samuc@LAPTOP-1UVA8F1I MINGW64 ~/Documents/atividade-6-samuel (dev)
$ git add .

samuc@LAPTOP-1UVA8F1I MINGW64 ~/Documents/atividade-6-samuel (dev)
$ git status
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        renamed:    arquivos2.js -> arquivos4.js


samuc@LAPTOP-1UVA8F1I MINGW64 ~/Documents/atividade-6-samuel (dev)
$  git commit -m "terceiro commit"
[dev 819b4f2] terceiro commit
 1 file changed, 0 insertions(+), 0 deletions(-)
 rename arquivos2.js => arquivos4.js (100%)

samuc@LAPTOP-1UVA8F1I MINGW64 ~/Documents/atividade-6-samuel (dev)
$ git add .

samuc@LAPTOP-1UVA8F1I MINGW64 ~/Documents/atividade-6-samuel (dev)
$  git commit -m "quarto commit"
[dev 083ceae] quarto commit
 1 file changed, 1 insertion(+)

samuc@LAPTOP-1UVA8F1I MINGW64 ~/Documents/atividade-6-samuel (dev)
$ git push -u origin dev
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 2 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (5/5), 485 bytes | 121.00 KiB/s, done.
Total 5 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 1 local object.
remote:
remote: Create a pull request for 'dev' on GitHub by visiting:
remote:      https://github.com/Shimu192/atividade-6-samuel/pull/new/dev
remote:
To https://github.com/Shimu192/atividade-6-samuel.git
 * [new branch]      dev -> dev
Branch 'dev' set up to track remote branch 'dev' from 'origin'.

samuc@LAPTOP-1UVA8F1I MINGW64 ~/Documents/atividade-6-samuel (dev)
$ git checkout -b "temp"
Switched to a new branch 'temp'

samuc@LAPTOP-1UVA8F1I MINGW64 ~/Documents/atividade-6-samuel (temp)
$ git status
On branch temp
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   arquivos3.js
        modified:   arquivos4.js

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        arquivos5.js

no changes added to commit (use "git add" and/or "git commit -a")

samuc@LAPTOP-1UVA8F1I MINGW64 ~/Documents/atividade-6-samuel (temp)
$ git add .

samuc@LAPTOP-1UVA8F1I MINGW64 ~/Documents/atividade-6-samuel (temp)
$  git commit -m "quinto commit"
[temp 196442a] quinto commit
 3 files changed, 3 insertions(+)
 create mode 100644 arquivos5.js

samuc@LAPTOP-1UVA8F1I MINGW64 ~/Documents/atividade-6-samuel (temp)
$ git push -u origin temp
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 2 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 253 bytes | 50.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'temp' on GitHub by visiting:
remote:      https://github.com/Shimu192/atividade-6-samuel/pull/new/temp
remote:
To https://github.com/Shimu192/atividade-6-samuel.git
 * [new branch]      temp -> temp
Branch 'temp' set up to track remote branch 'temp' from 'origin'.

samuc@LAPTOP-1UVA8F1I MINGW64 ~/Documents/atividade-6-samuel (temp)
$ git branch
  dev
  main
* temp

samuc@LAPTOP-1UVA8F1I MINGW64 ~/Documents/atividade-6-samuel (temp)
$ git merge dev
Already up to date.

samuc@LAPTOP-1UVA8F1I MINGW64 ~/Documents/atividade-6-samuel (temp)
$ git status
On branch temp
Your branch is up to date with 'origin/temp'.

nothing to commit, working tree clean

samuc@LAPTOP-1UVA8F1I MINGW64 ~/Documents/atividade-6-samuel (temp)
$ git push -u origin dev
Everything up-to-date
Branch 'dev' set up to track remote branch 'dev' from 'origin'.

samuc@LAPTOP-1UVA8F1I MINGW64 ~/Documents/atividade-6-samuel (temp)
$ git checkout dev
Switched to branch 'dev'
Your branch is up to date with 'origin/dev'.

samuc@LAPTOP-1UVA8F1I MINGW64 ~/Documents/atividade-6-samuel (dev)
$ git push -u origin dev
Everything up-to-date
Branch 'dev' set up to track remote branch 'dev' from 'origin'.

samuc@LAPTOP-1UVA8F1I MINGW64 ~/Documents/atividade-6-samuel (dev)
$  git commit -m "sexto commit"
On branch dev
Your branch is up to date with 'origin/dev'.

Changes not staged for commit:
  (use "git add/rm <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   arquivos1.js
        deleted:    arquivos4.js

no changes added to commit (use "git add" and/or "git commit -a")

samuc@LAPTOP-1UVA8F1I MINGW64 ~/Documents/atividade-6-samuel (dev)
$  git add .

samuc@LAPTOP-1UVA8F1I MINGW64 ~/Documents/atividade-6-samuel (dev)
$  git commit -m "sexto commit"
[dev e158171] sexto commit
 2 files changed, 1 insertion(+), 1 deletion(-)
 delete mode 100644 arquivos4.js

samuc@LAPTOP-1UVA8F1I MINGW64 ~/Documents/atividade-6-samuel (dev)
$ git merge main
Already up to date.

samuc@LAPTOP-1UVA8F1I MINGW64 ~/Documents/atividade-6-samuel (dev)
$ git status
On branch dev
Your branch is ahead of 'origin/dev' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean

samuc@LAPTOP-1UVA8F1I MINGW64 ~/Documents/atividade-6-samuel (dev)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 2 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 314 bytes | 7.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/Shimu192/atividade-6-samuel.git
   083ceae..e158171  dev -> dev

samuc@LAPTOP-1UVA8F1I MINGW64 ~/Documents/atividade-6-samuel (dev)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

samuc@LAPTOP-1UVA8F1I MINGW64 ~/Documents/atividade-6-samuel (main)
$ git tag -a v1.1 -m "versão de entrega"

samuc@LAPTOP-1UVA8F1I MINGW64 ~/Documents/atividade-6-samuel (main)
$ git tag
v1.0
v1.1

samuc@LAPTOP-1UVA8F1I MINGW64 ~/Documents/atividade-6-samuel (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")

samuc@LAPTOP-1UVA8F1I MINGW64 ~/Documents/atividade-6-samuel (main)
$ git add .

samuc@LAPTOP-1UVA8F1I MINGW64 ~/Documents/atividade-6-samuel (main)
$  git commit -m "arquivo readme"
[main 54ce073] arquivo readme
 1 file changed, 243 insertions(+)

samuc@LAPTOP-1UVA8F1I MINGW64 ~/Documents/atividade-6-samuel (main)
$ git status
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean

samuc@LAPTOP-1UVA8F1I MINGW64 ~/Documents/atividade-6-samuel (main)
$ git push -u origin main --tags
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 2 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 1.95 KiB | 285.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/Shimu192/atividade-6-samuel.git
   dd9a2a6..54ce073  main -> main
 * [new tag]         v1.1 -> v1.1
Branch 'main' set up to track remote branch 'main' from 'origin'.