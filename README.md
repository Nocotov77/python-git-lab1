# python-git-lab1
Терминал:
```
Microsoft Windows [Version 10.0.19045.5854]
(c) Корпорация Майкрософт (Microsoft Corporation). Все права защищены.

C:\Users\student-09-320.NCFU>ssh -T git@github.com
Enter passphrase for key 'C:\Users\student-09-320.NCFU/.ssh/id_ed25519':
Hi Nocotov77! You've successfully authenticated, but GitHub does not provide shell access.

C:\Users\student-09-320.NCFU>cd C:\Users\student-09-320.NCFU\Desktop\githere

C:\Users\student-09-320.NCFU\Desktop\githere>git status
On branch master

No commits yet

nothing to commit (create/copy files and use "git add" to track)

C:\Users\student-09-320.NCFU\Desktop\githere>git config --global user.name "Ваше Имя"

C:\Users\student-09-320.NCFU\Desktop\githere>git config --local user.name "Nikita"

C:\Users\student-09-320.NCFU\Desktop\githere>git config --local
error: no action specified

C:\Users\student-09-320.NCFU\Desktop\githere>git config --local show
error: key does not contain a section: show

C:\Users\student-09-320.NCFU\Desktop\githere>git config --help

C:\Users\student-09-320.NCFU\Desktop\githere>git config list --local
core.repositoryformatversion=0
core.filemode=false
core.bare=false
core.logallrefupdates=true
core.symlinks=false
core.ignorecase=true
user.name=Nikita

C:\Users\student-09-320.NCFU\Desktop\githere>git config --local user.email "chooryou2@gmail.com"

C:\Users\student-09-320.NCFU\Desktop\githere>git config --local core.editor "code --wait"

C:\Users\student-09-320.NCFU\Desktop\githere>git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        hello.py

nothing added to commit but untracked files present (use "git add" to track)

C:\Users\student-09-320.NCFU\Desktop\githere>git add hello.py

C:\Users\student-09-320.NCFU\Desktop\githere>git commit -m "Add initial hello.pt script"
[master (root-commit) b485591] Add initial hello.pt script
 1 file changed, 1 insertion(+)
 create mode 100644 hello.py

C:\Users\student-09-320.NCFU\Desktop\githere>git status
On branch master
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   hello.py

no changes added to commit (use "git add" and/or "git commit -a")

C:\Users\student-09-320.NCFU\Desktop\githere>git add.
git: 'add.' is not a git command. See 'git --help'.

The most similar command is
        add

C:\Users\student-09-320.NCFU\Desktop\githere>git add .

C:\Users\student-09-320.NCFU\Desktop\githere>git commit -m "Add a new print statement to hello.py"
[master 03eb5bb] Add a new print statement to hello.py
 1 file changed, 2 insertions(+), 1 deletion(-)

C:\Users\student-09-320.NCFU\Desktop\githere>git log --oneline
03eb5bb (HEAD -> master) Add a new print statement to hello.py
b485591 Add initial hello.pt script

C:\Users\student-09-320.NCFU\Desktop\githere>git checkout -b feature/greeting
Switched to a new branch 'feature/greeting'

C:\Users\student-09-320.NCFU\Desktop\githere>git status
On branch feature/greeting
nothing to commit, working tree clean

C:\Users\student-09-320.NCFU\Desktop\githere>git status
On branch feature/greeting
nothing to commit, working tree clean

C:\Users\student-09-320.NCFU\Desktop\githere>git status
On branch feature/greeting
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        greeting.py

nothing added to commit but untracked files present (use "git add" to track)

C:\Users\student-09-320.NCFU\Desktop\githere>git add .

C:\Users\student-09-320.NCFU\Desktop\githere>git commit -m "Add a new greeting module with user input"
[feature/greeting 83ea8cc] Add a new greeting module with user input
 1 file changed, 4 insertions(+)
 create mode 100644 greeting.py

C:\Users\student-09-320.NCFU\Desktop\githere>git checkout main
error: pathspec 'main' did not match any file(s) known to git

C:\Users\student-09-320.NCFU\Desktop\githere>git status
On branch feature/greeting
nothing to commit, working tree clean

C:\Users\student-09-320.NCFU\Desktop\githere>git checkout master
Switched to branch 'master'

C:\Users\student-09-320.NCFU\Desktop\githere>git status
On branch master
nothing to commit, working tree clean

C:\Users\student-09-320.NCFU\Desktop\githere>ls
"ls" не является внутренней или внешней
командой, исполняемой программой или пакетным файлом.

C:\Users\student-09-320.NCFU\Desktop\githere>dir
 Том в устройстве C не имеет метки.
 Серийный номер тома: 148F-0C80

 Содержимое папки C:\Users\student-09-320.NCFU\Desktop\githere

04.09.2025  12:13    <DIR>          .
04.09.2025  12:13    <DIR>          ..
04.09.2025  12:06                44 hello.py
               1 файлов             44 байт
               2 папок  118 800 089 088 байт свободно

C:\Users\student-09-320.NCFU\Desktop\githere>git merge feature/greeting
Updating 03eb5bb..83ea8cc
Fast-forward
 greeting.py | 4 ++++
 1 file changed, 4 insertions(+)
 create mode 100644 greeting.py

C:\Users\student-09-320.NCFU\Desktop\githere>git status
On branch master
nothing to commit, working tree clean

C:\Users\student-09-320.NCFU\Desktop\githere>dir
 Том в устройстве C не имеет метки.
 Серийный номер тома: 148F-0C80

 Содержимое папки C:\Users\student-09-320.NCFU\Desktop\githere

04.09.2025  12:14    <DIR>          .
04.09.2025  12:14    <DIR>          ..
04.09.2025  12:14                97 greeting.py
04.09.2025  12:06                44 hello.py
               2 файлов            141 байт
               2 папок  118 799 663 104 байт свободно

C:\Users\student-09-320.NCFU\Desktop\githere>git remote add origin git@github.com:ВАШ_АККАУНТ/python-git-lab1.git

C:\Users\student-09-320.NCFU\Desktop\githere>git remote add origin git@github.com:ВАШ_АККАУНТ/python-git-lab1.git
error: remote origin already exists.

C:\Users\student-09-320.NCFU\Desktop\githere>git remote add origin git@github.com:Nocotov77/python-git-lab1.git
error: remote origin already exists.

C:\Users\student-09-320.NCFU\Desktop\githere>git remote --help

C:\Users\student-09-320.NCFU\Desktop\githere>git remote remove origin

C:\Users\student-09-320.NCFU\Desktop\githere>git remote add origin git@github.com:Nocotov77/python-git-lab1.git

C:\Users\student-09-320.NCFU\Desktop\githere>git push -u origin master
Enter passphrase for key '/c/Users/student-09-320.NCFU/.ssh/id_ed25519':
To github.com:Nocotov77/python-git-lab1.git
 ! [rejected]        master -> master (fetch first)
error: failed to push some refs to 'github.com:Nocotov77/python-git-lab1.git'
hint: Updates were rejected because the remote contains work that you do not
hint: have locally. This is usually caused by another repository pushing to
hint: the same ref. If you want to integrate the remote changes, use
hint: 'git pull' before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

C:\Users\student-09-320.NCFU\Desktop\githere>git pull
Enter passphrase for key '/c/Users/student-09-320.NCFU/.ssh/id_ed25519':
remote: Enumerating objects: 5, done.
remote: Counting objects: 100% (5/5), done.
remote: Compressing objects: 100% (4/4), done.
remote: Total 5 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (5/5), 14.64 KiB | 428.00 KiB/s, done.
From github.com:Nocotov77/python-git-lab1
 * [new branch]      master     -> origin/master
There is no tracking information for the current branch.
Please specify which branch you want to merge with.
See git-pull(1) for details.

    git pull <remote> <branch>

If you wish to set tracking information for this branch you can do so with:

    git branch --set-upstream-to=origin/<branch> master


C:\Users\student-09-320.NCFU\Desktop\githere>git status
On branch master
nothing to commit, working tree clean

C:\Users\student-09-320.NCFU\Desktop\githere>git pull origin master
Enter passphrase for key '/c/Users/student-09-320.NCFU/.ssh/id_ed25519':
Enter passphrase for key '/c/Users/student-09-320.NCFU/.ssh/id_ed25519':
From github.com:Nocotov77/python-git-lab1
 * branch            master     -> FETCH_HEAD
fatal: refusing to merge unrelated histories

C:\Users\student-09-320.NCFU\Desktop\githere>git status
On branch master
nothing to commit, working tree clean

C:\Users\student-09-320.NCFU\Desktop\githere>git push -u origin master
Enter passphrase for key '/c/Users/student-09-320.NCFU/.ssh/id_ed25519':
Enter passphrase for key '/c/Users/student-09-320.NCFU/.ssh/id_ed25519':
To github.com:Nocotov77/python-git-lab1.git
 ! [rejected]        master -> master (non-fast-forward)
error: failed to push some refs to 'github.com:Nocotov77/python-git-lab1.git'
hint: Updates were rejected because the tip of your current branch is behind
hint: its remote counterpart. If you want to integrate the remote changes,
hint: use 'git pull' before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

C:\Users\student-09-320.NCFU\Desktop\githere>git pull
Enter passphrase for key '/c/Users/student-09-320.NCFU/.ssh/id_ed25519':
Enter passphrase for key '/c/Users/student-09-320.NCFU/.ssh/id_ed25519':
There is no tracking information for the current branch.
Please specify which branch you want to merge with.
See git-pull(1) for details.

    git pull <remote> <branch>

If you wish to set tracking information for this branch you can do so with:

    git branch --set-upstream-to=origin/<branch> master


C:\Users\student-09-320.NCFU\Desktop\githere>git pull origin master
Enter passphrase for key '/c/Users/student-09-320.NCFU/.ssh/id_ed25519':
From github.com:Nocotov77/python-git-lab1
 * branch            master     -> FETCH_HEAD
fatal: refusing to merge unrelated histories

C:\Users\student-09-320.NCFU\Desktop\githere>git pull origin master --allow-unrelated-histories
Enter passphrase for key '/c/Users/student-09-320.NCFU/.ssh/id_ed25519':
Enter passphrase for key '/c/Users/student-09-320.NCFU/.ssh/id_ed25519':
From github.com:Nocotov77/python-git-lab1
 * branch            master     -> FETCH_HEAD
hint: Waiting for your editor to close the file... code --wait: line 1: code: command not found
error: there was a problem with the editor 'code --wait'
Not committing merge; use 'git commit' to complete the merge.

C:\Users\student-09-320.NCFU\Desktop\githere>git status
On branch master
All conflicts fixed but you are still merging.
  (use "git commit" to conclude merge)

Changes to be committed:
        new file:   .gitignore
        new file:   LICENSE
        new file:   README.md


C:\Users\student-09-320.NCFU\Desktop\githere>git commit -m "merge repo"
[master 3cf3237] merge repo

C:\Users\student-09-320.NCFU\Desktop\githere>git status
On branch master
nothing to commit, working tree clean

C:\Users\student-09-320.NCFU\Desktop\githere>git push -u origin main
error: src refspec main does not match any
error: failed to push some refs to 'github.com:Nocotov77/python-git-lab1.git'

C:\Users\student-09-320.NCFU\Desktop\githere>git push -u origin master
Enter passphrase for key '/c/Users/student-09-320.NCFU/.ssh/id_ed25519':
Enumerating objects: 12, done.
Counting objects: 100% (12/12), done.
Delta compression using up to 12 threads
Compressing objects: 100% (7/7), done.
Writing objects: 100% (11/11), 1.18 KiB | 602.00 KiB/s, done.
Total 11 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To github.com:Nocotov77/python-git-lab1.git
   743608c..3cf3237  master -> master
branch 'master' set up to track 'origin/master'.

C:\Users\student-09-320.NCFU\Desktop\githere>git push origin feature/greeting
Enter passphrase for key '/c/Users/student-09-320.NCFU/.ssh/id_ed25519':
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote:
remote: Create a pull request for 'feature/greeting' on GitHub by visiting:
remote:      https://github.com/Nocotov77/python-git-lab1/pull/new/feature/greeting
remote:
To github.com:Nocotov77/python-git-lab1.git
 * [new branch]      feature/greeting -> feature/greeting

C:\Users\student-09-320.NCFU\Desktop\githere>python3 hello.py
Python
C:\Users\student-09-320.NCFU\Desktop\githere>python3 greeting.py
Python
C:\Users\student-09-320.NCFU\Desktop\githere>git status
On branch master
Your branch is up to date with 'origin/master'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        test_result.png

nothing added to commit but untracked files present (use "git add" to track)

C:\Users\student-09-320.NCFU\Desktop\githere>git add .

C:\Users\student-09-320.NCFU\Desktop\githere>git commit -m "Add test execution screenshot"
[master 753c16b] Add test execution screenshot
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 test_result.png

C:\Users\student-09-320.NCFU\Desktop\githere>git push origin master
Enter passphrase for key '/c/Users/student-09-320.NCFU/.ssh/id_ed25519':
Enter passphrase for key '/c/Users/student-09-320.NCFU/.ssh/id_ed25519':
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 66.02 KiB | 463.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To github.com:Nocotov77/python-git-lab1.git
   3cf3237..753c16b  master -> master

C:\Users\student-09-320.NCFU\Desktop\githere>
```