
Welcome to git.

im kamal
im kalyan, how are you buddy?


hey im from 1st branch.


PS C:\Users\kamalan\Desktop\git-learning> git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        Readme.md
        hello.js

nothing added to commit but untracked files present (use "git add" to track)
PS C:\Users\kamalan\Desktop\git-learning> git add Readme.md
PS C:\Users\kamalan\Desktop\git-learning> git add hello.js
PS C:\Users\kamalan\Desktop\git-learning> git commit -m "first commit"
[master (root-commit) 14f7dbc] first commit
 2 files changed, 2 insertions(+)
 create mode 100644 Readme.md
 create mode 100644 hello.js
PS C:\Users\kamalan\Desktop\git-learning> git status
On branch master
nothing to commit, working tree clean
PS C:\Users\kamalan\Desktop\git-learning> git log
commit 14f7dbc1856e399062e5540e0455a61b680d9e8d (HEAD -> master)
Author: kamalan2k4 <kmln2k4@gmail.com>
Date:   Mon Oct 7 13:43:11 2024 +0530

    first commit
PS C:\Users\kamalan\Desktop\git-learning> git checkout 14f7dbc1856e399062e5540e0455a61b680d9e8d     
Note: switching to '14f7dbc1856e399062e5540e0455a61b680d9e8d'.

You are in 'detached HEAD' state. You can look around, make experimental
changes and commit them, and you can discard any commits you make in this
state without impacting any branches by switching back to a branch.

If you want to create a new branch to retain commits you create, you may
do so (now or later) by using -c with the switch command. Example:

  git switch -c <new-branch-name>

Or undo this operation with:

  git switch -

Turn off this advice by setting config variable advice.detachedHead to false

HEAD is now at 14f7dbc first commit
PS C:\Users\kamalan\Desktop\git-learning> git checkout master
Switched to branch 'master'
PS C:\Users\kamalan\Desktop\git-learning> git add test.js
PS C:\Users\kamalan\Desktop\git-learning> git commit -m "added test.js"
[master d3799e8] added test.js
 1 file changed, 1 insertion(+)
 create mode 100644 test.js
PS C:\Users\kamalan\Desktop\git-learning> git status
On branch master
nothing to commit, working tree clean
PS C:\Users\kamalan\Desktop\git-learning> git log
commit d3799e81d49f0b42fcfe3b4ae24d71529167bbc2 (HEAD -> master)
Author: kamalan2k4 <kmln2k4@gmail.com>
Date:   Mon Oct 7 13:52:52 2024 +0530

    added test.js

commit 14f7dbc1856e399062e5540e0455a61b680d9e8d
Author: kamalan2k4 <kmln2k4@gmail.com>
Date:   Mon Oct 7 13:43:11 2024 +0530

    first commit
PS C:\Users\kamalan\Desktop\git-learning> git checkout 14f7dbc1856e399062e5540e0455a61b680d9e8d
Note: switching to '14f7dbc1856e399062e5540e0455a61b680d9e8d'.

You are in 'detached HEAD' state. You can look around, make experimental
changes and commit them, and you can discard any commits you make in this
state without impacting any branches by switching back to a branch.

If you want to create a new branch to retain commits you create, you may
do so (now or later) by using -c with the switch command. Example:

  git switch -c <new-branch-name>

Or undo this operation with:

  git switch -

Turn off this advice by setting config variable advice.detachedHead to false

HEAD is now at 14f7dbc first commit
PS C:\Users\kamalan\Desktop\git-learning> git -f checkout master
unknown option: -f
usage: git [-v | --version] [-h | --help] [-C <path>] [-c <name>=<value>]
           [--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
           [-p | --paginate | -P | --no-pager] [--no-replace-objects] [--bare]
           [--git-dir=<path>] [--work-tree=<path>] [--namespace=<name>]
           [--config-env=<name>=<envvar>] <command> [<args>]
PS C:\Users\kamalan\Desktop\git-learning> git checkout -f master
Previous HEAD position was 14f7dbc first commit
Switched to branch 'master'
PS C:\Users\kamalan\Desktop\git-learning> git branch -M main
PS C:\Users\kamalan\Desktop\git-learning> git remote add origin https://github.com/kamalan2k4/mastering-git.git
PS C:\Users\kamalan\Desktop\git-learning> git push -u origin main
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 8 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (7/7), 505 bytes | 168.00 KiB/s, done.
Total 7 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), done.
To https://github.com/kamalan2k4/mastering-git.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.
PS C:\Users\kamalan\Desktop\git-learning> git checkout -b 1st-branch
Switched to a new branch '1st-branch'
PS C:\Users\kamalan\Desktop\git-learning> git add .
PS C:\Users\kamalan\Desktop\git-learning> git commit -m "modify readme"
[1st-branch 3ff5152] modify readme
 1 file changed, 3 insertions(+), 1 deletion(-)
PS C:\Users\kamalan\Desktop\git-learning> git push --set-upstream origin 1st-branch
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 338 bytes | 112.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
remote: 
remote: Create a pull request for '1st-branch' on GitHub by visiting:
remote:      https://github.com/kamalan2k4/mastering-git/pull/new/1st-branch
remote:
To https://github.com/kamalan2k4/mastering-git.git
 * [new branch]      1st-branch -> 1st-branch
branch '1st-branch' set up to track 'origin/1st-branch'.
PS C:\Users\kamalan\Desktop\git-learning> git push
Everything up-to-date
PS C:\Users\kamalan\Desktop\git-learning> git pull
Already up to date.
PS C:\Users\kamalan\Desktop\git-learning> git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
PS C:\Users\kamalan\Desktop\git-learning> git pull
remote: Enumerating objects: 1, done.
remote: Counting objects: 100% (1/1), done.
remote: Total 1 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (1/1), 898 bytes | 128.00 KiB/s, done.
From https://github.com/kamalan2k4/mastering-git
   d3799e8..d7f9d22  main       -> origin/main
Updating d3799e8..d7f9d22
Fast-forward
 Readme.md | 4 +++-
 1 file changed, 3 insertions(+), 1 deletion(-)
PS C:\Users\kamalan\Desktop\git-learning> git branch kalyan
PS C:\Users\kamalan\Desktop\git-learning> git checkout -b kamal
Switched to a new branch 'kamal'
PS C:\Users\kamalan\Desktop\git-learning> git add .
PS C:\Users\kamalan\Desktop\git-learning> git commit "modify readme from kamal"
error: pathspec 'modify readme from kamal' did not match any file(s) known to git
PS C:\Users\kamalan\Desktop\git-learning> git commit -m "modify readme from kamal"
[kamal 862b93d] modify readme from kamal
 1 file changed, 3 insertions(+), 1 deletion(-)
PS C:\Users\kamalan\Desktop\git-learning> git checkout kalyan
Switched to branch 'kalyan'
PS C:\Users\kamalan\Desktop\git-learning> git add .
PS C:\Users\kamalan\Desktop\git-learning> git commit -m "dandanaka"
[kalyan 39afdd8] dandanaka
 1 file changed, 3 insertions(+), 1 deletion(-)
PS C:\Users\kamalan\Desktop\git-learning> git push -u origin kalyan
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 368 bytes | 184.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
remote: 
remote: Create a pull request for 'kalyan' on GitHub by visiting:
remote:      https://github.com/kamalan2k4/mastering-git/pull/new/kalyan
remote:
To https://github.com/kamalan2k4/mastering-git.git
 * [new branch]      kalyan -> kalyan
branch 'kalyan' set up to track 'origin/kalyan'.
PS C:\Users\kamalan\Desktop\git-learning> git checkout kamal
Switched to branch 'kamal'
PS C:\Users\kamalan\Desktop\git-learning> git push -u origin kamal
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 355 bytes | 118.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
remote: 
remote: Create a pull request for 'kamal' on GitHub by visiting:
remote:      https://github.com/kamalan2k4/mastering-git/pull/new/kamal
remote:
To https://github.com/kamalan2k4/mastering-git.git
 * [new branch]      kamal -> kamal
branch 'kamal' set up to track 'origin/kamal'.
PS C:\Users\kamalan\Desktop\git-learning> git merge main
Already up to date.
PS C:\Users\kamalan\Desktop\git-learning> git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
PS C:\Users\kamalan\Desktop\git-learning> git merge main
Already up to date.
PS C:\Users\kamalan\Desktop\git-learning> git pull
remote: Enumerating objects: 1, done.
remote: Counting objects: 100% (1/1), done.
remote: Total 1 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (1/1), 891 bytes | 74.00 KiB/s, done.
From https://github.com/kamalan2k4/mastering-git
   d7f9d22..eb858d8  main       -> origin/main
Updating d7f9d22..eb858d8
remote: Counting objects: 100% (1/1), done.
remote: Total 1 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (1/1), 891 bytes | 74.00 KiB/s, done.
From https://github.com/kamalan2k4/mastering-git
   d7f9d22..eb858d8  main       -> origin/main
Updating d7f9d22..eb858d8
Unpacking objects: 100% (1/1), 891 bytes | 74.00 KiB/s, done.
From https://github.com/kamalan2k4/mastering-git
   d7f9d22..eb858d8  main       -> origin/main
Updating d7f9d22..eb858d8
From https://github.com/kamalan2k4/mastering-git
   d7f9d22..eb858d8  main       -> origin/main
Updating d7f9d22..eb858d8
Fast-forward
   d7f9d22..eb858d8  main       -> origin/main
Updating d7f9d22..eb858d8
Fast-forward
 Readme.md | 4 +++-
Updating d7f9d22..eb858d8
Fast-forward
 Readme.md | 4 +++-
Fast-forward
 Readme.md | 4 +++-
 Readme.md | 4 +++-
 1 file changed, 3 insertions(+), 1 deletion(-)
PS C:\Users\kamalan\Desktop\git-learning> git checkout kamal
PS C:\Users\kamalan\Desktop\git-learning> git checkout kamal
Switched to branch 'kamal'
Your branch is up to date with 'origin/kamal'.
PS C:\Users\kamalan\Desktop\git-learning> git merge main
Auto-merging Readme.md
CONFLICT (content): Merge conflict in Readme.md
Automatic merge failed; fix conflicts and then commit the result.
PS C:\Users\kamalan\Desktop\git-learning> git checkout main
error: Your local changes to the following files would be overwritten by checkout:
        Readme.md
Please commit your changes or stash them before you switch branches.
Aborting
PS C:\Users\kamalan\Desktop\git-learning> git pull
error: You have not concluded your merge (MERGE_HEAD exists).
hint: Please, commit your changes before merging.
fatal: Exiting because of unfinished merge.
PS C:\Users\kamalan\Desktop\git-learning> git checkout kamal
Already on 'kamal'
M       Readme.md
Your branch is up to date with 'origin/kamal'.
PS C:\Users\kamalan\Desktop\git-learning> git add .                              
PS C:\Users\kamalan\Desktop\git-learning> git commit -m "resolved merge conflicts"
[kamal ecd46a3] resolved merge conflicts
 1 file changed, 2 insertions(+)
PS C:\Users\kamalan\Desktop\git-learning> git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
PS C:\Users\kamalan\Desktop\git-learning> git pull
remote: Enumerating objects: 8, done.
remote: Counting objects: 100% (8/8), done.
remote: Compressing objects: 100% (4/4), done.
remote: Total 4 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (4/4), 1.91 KiB | 78.00 KiB/s, done.
From https://github.com/kamalan2k4/mastering-git
   eb858d8..0a71788  main       -> origin/main
   862b93d..949c55d  kamal      -> origin/kamal
Updating eb858d8..0a71788
Fast-forward
 Readme.md | 5 ++++-
 1 file changed, 4 insertions(+), 1 deletion(-)
PS C:\Users\kamalan\Desktop\git-learning> git checkout kamal
Switched to branch 'kamal'
Your branch and 'origin/kamal' have diverged,
and have 1 and 3 different commits each, respectively.
  (use "git pull" to merge the remote branch into yours)
PS C:\Users\kamalan\Desktop\git-learning> git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
PS C:\Users\kamalan\Desktop\git-learning> git checkout kalyan
Switched to branch 'kalyan'
Your branch is up to date with 'origin/kalyan'.
PS C:\Users\kamalan\Desktop\git-learning> git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
PS C:\Users\kamalan\Desktop\git-learning> git add .
PS C:\Users\kamalan\Desktop\git-learning> git commit -m "kamal added"
[main f665fcf] kamal added
 1 file changed, 2 insertions(+), 1 deletion(-)
PS C:\Users\kamalan\Desktop\git-learning> git add .
PS C:\Users\kamalan\Desktop\git-learning> git commit -m "kalyan added"
[main 998d3f8] kalyan added
 1 file changed, 2 insertions(+), 1 deletion(-)
PS C:\Users\kamalan\Desktop\git-learning> git add .
PS C:\Users\kamalan\Desktop\git-learning> git commit -m "venkat added"
[main 0af3c48] venkat added
 1 file changed, 2 insertions(+), 1 deletion(-)
PS C:\Users\kamalan\Desktop\git-learning> git log
commit 0af3c48cd1c7b48b43a6dd7fc2361728983c8b1e (HEAD -> main)
Author: kamalan2k4 <kmln2k4@gmail.com>
Date:   Mon Oct 7 15:16:54 2024 +0530

    venkat added

commit 998d3f856841b1b50b9850390d3d6d00c03da125
Author: kamalan2k4 <kmln2k4@gmail.com>
Date:   Mon Oct 7 15:16:22 2024 +0530

    kalyan added

commit f665fcfe902fff23252e850b687a39e6d7598267
Author: kamalan2k4 <kmln2k4@gmail.com>
Date:   Mon Oct 7 15:15:57 2024 +0530

    kamal added

commit 0a717881c5692955c7888009f4725db01106009d (origin/main)
Merge: eb858d8 949c55d
Author: kamal <117959444+kamalan2k4@users.noreply.github.com>
Date:   Mon Oct 7 15:00:45 2024 +0530

    Merge pull request #2 from kamalan2k4/kamal

    modify readme from kamal

commit 949c55db4524e071fc24ca3242926f3e17dddc65 (origin/kamal)
Merge: 862b93d eb858d8
Author: kamal <117959444+kamalan2k4@users.noreply.github.com>
Date:   Mon Oct 7 15:00:21 2024 +0530

    Merge branch 'main' into kamal

commit eb858d88f176d0ae1fde233699a8af5435ae65b7
Merge: d7f9d22 39afdd8
Author: kamal <117959444+kamalan2k4@users.noreply.github.com>
Date:   Mon Oct 7 14:46:12 2024 +0530

    Merge pull request #3 from kamalan2k4/kalyan

    dandanaka

commit 39afdd88b4e567e3de40870430dec25fd842ce6b (origin/kalyan, kalyan)
Author: kamalan2k4 <kmln2k4@gmail.com>
Date:   Mon Oct 7 14:42:09 2024 +0530

    dandanaka

commit 862b93d18e622aec3c1d0d37f26bdb332f87d325
Author: kamalan2k4 <kmln2k4@gmail.com>
Date:   Mon Oct 7 14:40:32 2024 +0530

    modify readme from kamal

commit d7f9d22ffbaf9b2c8b645465451f3e69b07da0bd
Merge: d3799e8 3ff5152
Author: kamal <117959444+kamalan2k4@users.noreply.github.com>
Date:   Mon Oct 7 14:18:55 2024 +0530

    Merge pull request #1 from kamalan2k4/1st-branch

    modify readme

commit 3ff5152a89faa5939d7a3608a636686e2c773d92 (origin/1st-branch, 1st-branch)
Author: kamalan2k4 <kmln2k4@gmail.com>
Date:   Mon Oct 7 14:10:21 2024 +0530

    modify readme

commit d3799e81d49f0b42fcfe3b4ae24d71529167bbc2
Author: kamalan2k4 <kmln2k4@gmail.com>
Date:   Mon Oct 7 13:52:52 2024 +0530

    added test.js

commit 14f7dbc1856e399062e5540e0455a61b680d9e8d
Author: kamalan2k4 <kmln2k4@gmail.com>
Date:   Mon Oct 7 13:43:11 2024 +0530

    first commit
PS C:\Users\kamalan\Desktop\git-learning> git reset f665fcfe902fff23252e850b687a39e6d7598267
Unstaged changes after reset:
M       hello.js
PS C:\Users\kamalan\Desktop\git-learning> git log
commit f665fcfe902fff23252e850b687a39e6d7598267 (HEAD -> main)
Author: kamalan2k4 <kmln2k4@gmail.com>
Date:   Mon Oct 7 15:15:57 2024 +0530

    kamal added

commit 0a717881c5692955c7888009f4725db01106009d (origin/main)
Merge: eb858d8 949c55d
Author: kamal <117959444+kamalan2k4@users.noreply.github.com>
Date:   Mon Oct 7 15:00:45 2024 +0530

    Merge pull request #2 from kamalan2k4/kamal

    modify readme from kamal

commit 949c55db4524e071fc24ca3242926f3e17dddc65 (origin/kamal)
Merge: 862b93d eb858d8
Author: kamal <117959444+kamalan2k4@users.noreply.github.com>
Date:   Mon Oct 7 15:00:21 2024 +0530

    Merge branch 'main' into kamal

commit eb858d88f176d0ae1fde233699a8af5435ae65b7
Merge: d7f9d22 39afdd8
Author: kamal <117959444+kamalan2k4@users.noreply.github.com>
Date:   Mon Oct 7 14:46:12 2024 +0530

    Merge pull request #3 from kamalan2k4/kalyan

    dandanaka

commit 39afdd88b4e567e3de40870430dec25fd842ce6b (origin/kalyan, kalyan)
Author: kamalan2k4 <kmln2k4@gmail.com>
Date:   Mon Oct 7 14:42:09 2024 +0530

    dandanaka

commit 862b93d18e622aec3c1d0d37f26bdb332f87d325
Author: kamalan2k4 <kmln2k4@gmail.com>
Date:   Mon Oct 7 14:40:32 2024 +0530

    modify readme from kamal

commit d7f9d22ffbaf9b2c8b645465451f3e69b07da0bd
Merge: d3799e8 3ff5152
Author: kamal <117959444+kamalan2k4@users.noreply.github.com>
Date:   Mon Oct 7 14:18:55 2024 +0530

    Merge pull request #1 from kamalan2k4/1st-branch

    modify readme

commit 3ff5152a89faa5939d7a3608a636686e2c773d92 (origin/1st-branch, 1st-branch)
Author: kamalan2k4 <kmln2k4@gmail.com>
Date:   Mon Oct 7 14:10:21 2024 +0530

    modify readme

commit d3799e81d49f0b42fcfe3b4ae24d71529167bbc2
Author: kamalan2k4 <kmln2k4@gmail.com>
Date:   Mon Oct 7 13:52:52 2024 +0530

    added test.js

commit 14f7dbc1856e399062e5540e0455a61b680d9e8d
Author: kamalan2k4 <kmln2k4@gmail.com>
Date:   Mon Oct 7 13:43:11 2024 +0530

    first commit
PS C:\Users\kamalan\Desktop\git-learning> git add .
PS C:\Users\kamalan\Desktop\git-learning> git pull  
Already up to date.
PS C:\Users\kamalan\Desktop\git-learning> git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 329 bytes | 109.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/kamalan2k4/mastering-git.git
   0a71788..f665fcf  main -> main
PS C:\Users\kamalan\Desktop\git-learning> git add .
PS C:\Users\kamalan\Desktop\git-learning> git commit -m "trying out revert"
[main 01d6974] trying out revert
 1 file changed, 2 insertions(+), 1 deletion(-)
PS C:\Users\kamalan\Desktop\git-learning> git log
commit 01d6974a5b4dc14fa2243d499941805da63971a5 (HEAD -> main)
Author: kamalan2k4 <kmln2k4@gmail.com>
Date:   Mon Oct 7 15:30:18 2024 +0530

    trying out revert

commit f665fcfe902fff23252e850b687a39e6d7598267 (origin/main)
Author: kamalan2k4 <kmln2k4@gmail.com>
Date:   Mon Oct 7 15:15:57 2024 +0530

    kamal added
PS C:\Users\kamalan\Desktop\git-learning> git revert f665fcfe902fff23252e850b687a39e6d7598267
Auto-merging hello.js
CONFLICT (content): Merge conflict in hello.js
error: could not revert f665fcf... kamal added
hint: After resolving the conflicts, mark them with
hint: "git add/rm <pathspec>", then run
hint: "git revert --continue".
hint: You can instead skip this commit with "git revert --skip".
hint: To abort and get back to the state before "git revert",
hint: run "git revert --abort".
PS C:\Users\kamalan\Desktop\git-learning> git revert --continue
error: Committing is not possible because you have unmerged files.
hint: Fix them up in the work tree, and then use 'git add/rm <file>'
hint: as appropriate to mark resolution and make a commit.
fatal: Exiting because of an unresolved conflict.
U       hello.js
PS C:\Users\kamalan\Desktop\git-learning> git add .
PS C:\Users\kamalan\Desktop\git-learning> git revert --continue
hint: Waiting for your editor to close the file...

Press ENTER or type command to continue
[main 7b646dc] Revert "kamal added"
 1 file changed, 2 insertions(+), 1 deletion(-)
PS C:\Users\kamalan\Desktop\git-learning> git log
commit 7b646dc70d57ba9e5fab08358cbdcdc29dea3992 (HEAD -> main)
Author: kamalan2k4 <kmln2k4@gmail.com>
Date:   Mon Oct 7 15:33:35 2024 +0530

    Revert "kamal added"

    This reverts commit f665fcfe902fff23252e850b687a39e6d7598267.

commit 01d6974a5b4dc14fa2243d499941805da63971a5
Author: kamalan2k4 <kmln2k4@gmail.com>
Date:   Mon Oct 7 15:30:18 2024 +0530

    trying out revert

commit f665fcfe902fff23252e850b687a39e6d7598267 (origin/main)
Author: kamalan2k4 <kmln2k4@gmail.com>
Date:   Mon Oct 7 15:15:57 2024 +0530

    kamal added

commit 0a717881c5692955c7888009f4725db01106009d
Merge: eb858d8 949c55d
Author: kamal <117959444+kamalan2k4@users.noreply.github.com>
Date:   Mon Oct 7 15:00:45 2024 +0530

    Merge pull request #2 from kamalan2k4/kamal

    modify readme from kamal

PS C:\Users\kamalan\Desktop\git-learning> git satsh
git: 'satsh' is not a git command. See 'git --help'.

The most similar command is
        stash
PS C:\Users\kamalan\Desktop\git-learning> git stash
Saved working directory and index state WIP on main: 7b646dc Revert "kamal added"
PS C:\Users\kamalan\Desktop\git-learning> git add .
PS C:\Users\kamalan\Desktop\git-learning> git commit -m "save the day"
[main 4983acc] save the day
 1 file changed, 1 insertion(+), 1 deletion(-)
PS C:\Users\kamalan\Desktop\git-learning> git stash list
stash@{0}: WIP on main: 7b646dc Revert "kamal added"
PS C:\Users\kamalan\Desktop\git-learning> git stash apply stash@{0}
error: unknown switch `e'
usage: git stash apply [--index] [-q | --quiet] [<stash>]

    -q, --quiet           be quiet, only report errors
    --index               attempt to recreate the index

PS C:\Users\kamalan\Desktop\git-learning> git stash apply stash@{0}
error: unknown switch `e'
usage: git stash apply [--index] [-q | --quiet] [<stash>]

    -q, --quiet           be quiet, only report errors
    --index               attempt to recreate the index

PS C:\Users\kamalan\Desktop\git-learning> git stash list
>>
stash@{0}: WIP on main: 7b646dc Revert "kamal added"
PS C:\Users\kamalan\Desktop\git-learning> git stash apply stash@{0}
error: unknown switch `e'
usage: git stash apply [--index] [-q | --quiet] [<stash>]

    -q, --quiet           be quiet, only report errors
    --index               attempt to recreate the index

PS C:\Users\kamalan\Desktop\git-learning> git stash apply "stash@{0}"
Auto-merging hello.js
CONFLICT (content): Merge conflict in hello.js
On branch main
Your branch is ahead of 'origin/main' by 3 commits.
  (use "git push" to publish your local commits)

Unmerged paths:
  (use "git restore --staged <file>..." to unstage)
  (use "git add <file>..." to mark resolution)
        both modified:   hello.js

no changes added to commit (use "git add" and/or "git commit -a")
PS C:\Users\kamalan\Desktop\git-learning> git add .
PS C:\Users\kamalan\Desktop\git-learning> git commit -m "final"  
[main 18682c9] final
 1 file changed, 5 insertions(+)
PS C:\Users\kamalan\Desktop\git-learning> git push -u origin main
Enumerating objects: 14, done.
Counting objects: 100% (14/14), done.
Delta compression using up to 8 threads
Compressing objects: 100% (11/11), done.
Writing objects: 100% (12/12), 1.33 KiB | 170.00 KiB/s, done.
Total 12 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/kamalan2k4/mastering-git.git
   f665fcf..18682c9  main -> main
branch 'main' set up to track 'origin/main'.
PS C:\Users\kamalan\Desktop\git-learning>