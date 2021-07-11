#Github

Learning github

Tutorial link: https://www.youtube.com/watch?v=SWYqp7iY_Tc

##Git Bash Commands:
KIIT@CSE1805094 MINGW64 ~/desktop/myapp
$ git init
Initialized empty Git repository in C:/Users/KIIT/Desktop/myapp/.git/

KIIT@CSE1805094 MINGW64 ~/desktop/myapp (master)
$ git config
usage: git config [<options>]

Config file location
--global use global config file
--system use system config file
--local use repository config file  
 --worktree use per-worktree config file  
 -f, --file <file> use given config file
--blob <blob-id> read config from given blob object

Action
--get get value: name [value-regex]
--get-all get all values: key [value-regex]
--get-regexp get values for regexp: name-regex [value-regex]  
 --get-urlmatch get value specific for the URL: section[.var] URL
--replace-all replace all matching variables: name value [value_regex]
--add add a new variable: name value
--unset remove a variable: name [value-regex]
--unset-all remove all matches: name [value-regex]
--rename-section rename section: old-name new-name
--remove-section remove a section: name
-l, --list list all
-e, --edit open an editor
--get-color find the color configured: slot [default]  
 --get-colorbool find the color setting: slot [stdout-is-tty]

Type
-t, --type <> value is given this type
--bool value is "true" or "false"
--int value is decimal number
--bool-or-int value is --bool or --int
--bool-or-str value is --bool or string
--path value is a path (file or directory name)
--expiry-date value is an expiry date

Other
-z, --null terminate values with NUL byte
--name-only show variable names only
--includes respect include directives on lookup
--show-origin show origin of config (file, standard input, blob, command line)
--show-scope show scope of config (worktree, local, global, system, command)
--default <value> with --get, use default value when missing entry

KIIT@CSE1805094 MINGW64 ~/desktop/myapp (master)
$ git config --global user.name 'Adity Kumar'

KIIT@CSE1805094 MINGW64 ~/desktop/myapp (master)
$ git config --global user.name 'Aditya Kumar'

KIIT@CSE1805094 MINGW64 ~/desktop/myapp (master)
$ git config --global user.email 'ak19992017@gmail.com'

KIIT@CSE1805094 MINGW64 ~/desktop/myapp (master)
$ git add index.html

KIIT@CSE1805094 MINGW64 ~/desktop/myapp (master)
$ git status
On branch master

No commits yet

Changes to be committed:
(use "git rm --cached <file>..." to unstage)
new file: index.html

Untracked files:
(use "git add <file>..." to include in what will be committed)
app.js

KIIT@CSE1805094 MINGW64 ~/desktop/myapp (master)
$ git rm --cached index.html
rm 'index.html'

KIIT@CSE1805094 MINGW64 ~/desktop/myapp (master)
$ git status
On branch master

No commits yet

Untracked files:
(use "git add <file>..." to include in what will be committed)
app.js
index.html

nothing added to commit but untracked files present (use "git add" to track)

KIIT@CSE1805094 MINGW64 ~/desktop/myapp (master)
$ git add \*.html

KIIT@CSE1805094 MINGW64 ~/desktop/myapp (master)
$ git status
On branch master

No commits yet

Changes to be committed:
(use "git rm --cached <file>..." to unstage)
new file: index.html

Untracked files:
(use "git add <file>..." to include in what will be committed)
app.js

KIIT@CSE1805094 MINGW64 ~/desktop/myapp (master)
$ git rm --cached index.html
rm 'index.html'

KIIT@CSE1805094 MINGW64 ~/desktop/myapp (master)
$ git add .

KIIT@CSE1805094 MINGW64 ~/desktop/myapp (master)
$ git status
On branch master

No commits yet

Changes to be committed:
(use "git rm --cached <file>..." to unstage)
new file: app.js
new file: index.html

KIIT@CSE1805094 MINGW64 ~/desktop/myapp (master)
$ git status
On branch master

No commits yet

Changes to be committed:
(use "git rm --cached <file>..." to unstage)
new file: app.js
new file: index.html

Changes not staged for commit:
(use "git add <file>..." to update what will be committed)
(use "git restore <file>..." to discard changes in working directory)  
 modified: index.html

KIIT@CSE1805094 MINGW64 ~/desktop/myapp (master)
$ git add .

KIIT@CSE1805094 MINGW64 ~/desktop/myapp (master)
$ git status
On branch master

No commits yet

Changes to be committed:
(use "git rm --cached <file>..." to unstage)
new file: app.js
new file: index.html

KIIT@CSE1805094 MINGW64 ~/desktop/myapp (master)
$ git commit
[master (root-commit) fbde64c] Initial commit
2 files changed, 15 insertions(+)
create mode 100644 app.js
create mode 100644 index.html

KIIT@CSE1805094 MINGW64 ~/desktop/myapp (master)
$ git status
On branch master
nothing to commit, working tree clean

KIIT@CSE1805094 MINGW64 ~/desktop/myapp (master)
$ git status
On branch master
Changes not staged for commit:
(use "git add <file>..." to update what will be committed)
(use "git restore <file>..." to discard changes in working directory)

no changes added to commit (use "git add" and/or "git commit -a") t commit -a")

KIIT@CSE1805094 MINGW64 ~/desktop/myapp (master)  
$ git add .

KIIT@CSE1805094 MINGW64 ~/desktop/myapp (master)  
$ git commit -m 'Changed app.js'
[master 368aa03] Changed app.js
1 file changed, 1 insertion(+)

KIIT@CSE1805094 MINGW64 ~/desktop/myapp (master)  
$ touch .gitignore

KIIT@CSE1805094 MINGW64 ~/desktop/myapp (master)  
$ touch log.txt

KIIT@CSE1805094 MINGW64 ~/desktop/myapp (master)  
$ git add .

KIIT@CSE1805094 MINGW64 ~/desktop/myapp (master)  
$ git status
On branch master
Changes to be committed:
(use "git restore --staged <file>..." to unstage)
new file: .gitignore

KIIT@CSE1805094 MINGW64 ~/desktop/myapp (master)  
$ mkdir dir1

KIIT@CSE1805094 MINGW64 ~/desktop/myapp (master)  
$ cd dir1 && touch app1.js

KIIT@CSE1805094 MINGW64 ~/desktop/myapp/dir1 (master)
$ cd .

KIIT@CSE1805094 MINGW64 ~/desktop/myapp/dir1 (master)
$ cd ..

KIIT@CSE1805094 MINGW64 ~/desktop/myapp (master)  
$ mkdir dir2 && cd dir2 && touch app2.js

KIIT@CSE1805094 MINGW64 ~/desktop/myapp/dir2 (master)
$ git add .
The following paths are ignored by one of your .gitignore files:
dir2
hint: Use -f if you really want to add them.  
hint: Turn this message off by running
hint: "git config advice.addIgnoredFile false"

KIIT@CSE1805094 MINGW64 ~/desktop/myapp/dir2 (master)
$ git status
On branch master
Changes to be committed:
(use "git restore --staged <file>..." to unstage)
new file: ../.gitignore

Changes not staged for commit:
(use "git add <file>..." to update what will be committed)
(use "git restore <file>..." to discard changes in working directory)
modified: ../.gitignore

Untracked files:
(use "git add <file>..." to include in what will be committed)
../dir1/

KIIT@CSE1805094 MINGW64 ~/desktop/myapp/dir2 (master)
$ cd ..

KIIT@CSE1805094 MINGW64 ~/desktop/myapp (master)  
$ git add .

KIIT@CSE1805094 MINGW64 ~/desktop/myapp (master)  
$ git status
On branch master
Changes to be committed:
(use "git restore --staged <file>..." to unstage)
new file: .gitignore
new file: dir1/app1.js

KIIT@CSE1805094 MINGW64 ~/desktop/myapp (master)  
$ git branch login

KIIT@CSE1805094 MINGW64 ~/desktop/myapp (master)  
$ git status
On branch master
Changes to be committed:
(use "git restore --staged <file>..." to unstage)
new file: .gitignore
new file: dir1/app1.js

KIIT@CSE1805094 MINGW64 ~/desktop/myapp (master)  
$ git commit -m 'another change'
[master c8f0462] another change
2 files changed, 3 insertions(+)
create mode 100644 .gitignore
create mode 100644 dir1/app1.js

KIIT@CSE1805094 MINGW64 ~/desktop/myapp (master)  
$ git status
On branch master
nothing to commit, working tree clean

KIIT@CSE1805094 MINGW64 ~/desktop/myapp (master)  
$ git checkout login
Switched to branch 'login'

KIIT@CSE1805094 MINGW64 ~/desktop/myapp (login)  
$ touch login.html

KIIT@CSE1805094 MINGW64 ~/desktop/myapp (login)  
$ git add .

KIIT@CSE1805094 MINGW64 ~/desktop/myapp (login)  
$ git commit -m 'login form'
[login a79c5c5] login form
4 files changed, 4 insertions(+)
create mode 100644 dir2/app2.js
create mode 100644 log.txt
create mode 100644 login.html

KIIT@CSE1805094 MINGW64 ~/desktop/myapp (login)  
$ git checkout master
Switched to branch 'master'

KIIT@CSE1805094 MINGW64 ~/desktop/myapp (master)  
$ git merge login
Merge made by the 'recursive' strategy.
dir2/app2.js | 1 +
index.html | 1 +
log.txt | 1 +
login.html | 1 +
4 files changed, 4 insertions(+)
create mode 100644 dir2/app2.js
create mode 100644 log.txt
create mode 100644 login.html

KIIT@CSE1805094 MINGW64 ~/desktop/myapp (master)  
$ git remote

KIIT@CSE1805094 MINGW64 ~/desktop/myapp (master)  
$ git remote add origin git@github.com:ak19992017/clock_app.git

KIIT@CSE1805094 MINGW64 ~/desktop/myapp (master)  
$ git remote
origin

KIIT@CSE1805094 MINGW64 ~/desktop/myapp (master)  
$ git push -u origin main
error: src refspec main does not match any
error: failed to push some refs to 'github.com:ak19992017/clock_app.git'

KIIT@CSE1805094 MINGW64 ~/desktop/myapp (master)  
$ git status
On branch master
nothing to commit, working tree clean

KIIT@CSE1805094 MINGW64 ~/desktop/myapp (master)  
$ git remote
origin

KIIT@CSE1805094 MINGW64 ~/desktop/myapp (master)  
$ git push -u origin main
error: src refspec main does not match any
error: failed to push some refs to 'github.com:ak19992017/clock_app.git'

KIIT@CSE1805094 MINGW64 ~/desktop/myapp (master)  
$ git show-ref
a79c5c5b7b418f21d24b4781a1ca7c56206ebbb9 refs/heads/login
b09b6fa3732465fb3ded8d07a362dd72dba271d2 refs/heads/master

KIIT@CSE1805094 MINGW64 ~/desktop/myapp (master)  
$ git push -u origin master
git@github.com: Permission denied (publickey).
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.

KIIT@CSE1805094 MINGW64 ~/desktop/myapp (master)  
$ git remote add origin https://github.com/ak19992017/clock_app.git
fatal: remote origin already exists.

KIIT@CSE1805094 MINGW64 ~/desktop/myapp (master)  
$ git remote add rigin https://github.com/ak19992017/clock_app.git

KIIT@CSE1805094 MINGW64 ~/desktop/myapp (master)  
$ git remote
origin
rigin

KIIT@CSE1805094 MINGW64 ~/desktop/myapp (master)  
$ git push -u rigin main
error: src refspec main does not match any
error: failed to push some refs to 'https://github.com/ak19992017/clock_app.git'

KIIT@CSE1805094 MINGW64 ~/desktop/myapp (master)  
$ git push -u origin master
git@github.com: Permission denied (publickey).
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.

KIIT@CSE1805094 MINGW64 ~/desktop/myapp (master)  
$ git push -u rigin master
Enumerating objects: 20, done.
Counting objects: 100% (20/20), done.
Delta compression using up to 8 threads
Compressing objects: 100% (12/12), done.
Writing objects: 100% (20/20), 1.66 KiB | 283.00 KiB/s, done.
Total 20 (delta 4), reused 0 (delta 0), pack-reused
0
remote: Resolving deltas: 100% (4/4), done.
To https://github.com/ak19992017/clock_app.git

- [new branch] master -> master
  Branch 'master' set up to track remote branch 'master' from 'rigin'.

KIIT@CSE1805094 MINGW64 ~/desktop/myapp (master)  
$ touch README.md

KIIT@CSE1805094 MINGW64 ~/desktop/myapp (master)  
$ git add .

KIIT@CSE1805094 MINGW64 ~/desktop/myapp (master)  
$ git commit -m 'Added README.md'
[master e503500] Added README.md
1 file changed, 5 insertions(+)
create mode 100644 README.md

KIIT@CSE1805094 MINGW64 ~/desktop/myapp (master)  
$ git push
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 357 bytes | 357.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: This repository moved. Please use the new location:
remote: https://github.com/ak19992017/learning_git.git
To https://github.com/ak19992017/clock_app.git
b09b6fa..e503500 master -> master

KIIT@CSE1805094 MINGW64 ~/desktop/myapp (master)  
$ cd ..

KIIT@CSE1805094 MINGW64 ~/desktop
$ git clone https://github.com/ak19992017/learning_git.git
Cloning into 'learning_git'...
remote: Enumerating objects: 23, done.
remote: Counting objects: 100% (23/23), done.  
remote: Compressing objects: 100% (10/10), done.  
remote: Total 23 (delta 5), reused 23 (delta 5), pack-reused 0
Receiving objects: 100% (23/23), done.
Resolving deltas: 100% (5/5), done.

KIIT@CSE1805094 MINGW64 ~/desktop
$ git pull
fatal: not a git repository (or any of the parent directories): .git

KIIT@CSE1805094 MINGW64 ~/desktop
$
