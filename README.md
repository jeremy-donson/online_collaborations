# online_collaborations
open source music stems

STUFF I DID ON THE COMMAND LINE
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

$ git log

$ git status

$ git push

$ git status
```
