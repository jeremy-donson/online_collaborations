# online_collaborations
open source music stems

STUFF I DID ON THE COMMAND LINE

[FIRST CONFIGURE LOCAL GIT](https://git-scm.com/book/en/v2/Getting-Started-First-Time-Git-Setup
)
```
$ git clone https://github.com/jeremy-donson/online_collaborations.git
Cloning into 'online_collaborations'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (3/3), done.

$ cd online_collaborations/
$ mkdir code
$ mkdir music
$ echo 'echo "Hello World!"' > code/hello.sh
$ git status
On branch master
Your branch is up to date with 'origin/master'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)

	code/

nothing added to commit but untracked files present (use "git add" to track)

$ bash code/hello.sh 
Hello World!

$ mkdir code/tests/

$ echo 'bash ../hello.sh' > code/tests/hello_test.sh

$ git status
On branch master
Your branch is up to date with 'origin/master'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)

	code/

nothing added to commit but untracked files present (use "git add" to track)

$ pwd
/Users/macbookair/projects/dseiden/online_collaborations

$ git add .

$ git status
On branch master
Your branch is up to date with 'origin/master'.

Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

	new file:   code/hello.sh
	new file:   code/tests/hello_test.sh

$ git commit -m 'Added some folders + a code script + a code test script.'
[master 45c5c2c] Added some folders + a code script + a code test script.
 2 files changed, 2 insertions(+)
 create mode 100644 code/hello.sh
 create mode 100644 code/tests/hello_test.sh

$ vi README.md 

$ git status
On branch master
Your branch is ahead of 'origin/master' by 1 commit.
  (use "git push" to publish your local commits)

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

	modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")

$ git add .
$ git commit -m 'Recorded my steps in README.md.'
[master 7c80603] Recorded my steps in README.md.
 1 file changed, 72 insertions(+)

$ git status
On branch master
Your branch is ahead of 'origin/master' by 2 commits.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean

$ git log
commit 7c806039e70e4b03287510c9f8613a248ba9738f (HEAD -> master)
Author: Jeremy Donson <jjdonson@gmail.com>
Date:   Tue Jul 16 20:23:55 2019 -0400

    Recorded my steps in README.md.

commit 45c5c2c3e8e40a0acb8ff8cf3f1a8682f7762cef
Author: Jeremy Donson <jjdonson@gmail.com>
Date:   Tue Jul 16 20:19:02 2019 -0400

    Added some folders + a code script + a code test script.

commit c48929ad7f368a0af57ac770782f388148c8a2fa (origin/master, origin/HEAD)
Author: danseiden <52935131+danseiden@users.noreply.github.com>
Date:   Mon Jul 15 15:52:09 2019 -0400

    Initial commit

$ git push
Username for 'https://github.com': jeremy-donson
Password for 'https://jeremy-donson@github.com': 
Enumerating objects: 11, done.
Counting objects: 100% (11/11), done.
Delta compression using up to 4 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (9/9), 1.33 KiB | 681.00 KiB/s, done.
Total 9 (delta 0), reused 0 (delta 0)
To https://github.com/jeremy-donson/online_collaborations.git
   c48929a..7c80603  master -> master

$ git status
On branch master
Your branch is up to date with 'origin/master'.

nothing to commit, working tree clean


```
