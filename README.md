# Gym Git Exercise Solutions

This README file contains my solutions for most of the bundles of the Git exercises provided to us by our coaches, in person of Tresor Manzi and Souvede Inshuti from the gym.

## Table of Contents

- [Bundle 1](#bundle-1)
  - [Exercise 1](#exercise-1)
  - [Exercise 2](#exercise-2)

## Bundle 1

### Exercise 1

```bash
oplanos-mbp:gym-git-exercise-solutions oplanojamesmulbah$ git status
fatal: not a git repository (or any of the parent directories): .git

oplanos-mbp:gym-git-exercise-solutions oplanojamesmulbah$ git init
Initialized empty Git repository in /Users/oplanojamesmulbah/gym-git-exercise-solutions/.git/

oplanos-mbp:gym-git-exercise-solutions oplanojamesmulbah$ git status
On branch main
No commits yet
nothing to commit (create/copy files and use "git add" to track)

oplanos-mbp:gym-git-exercise-solutions oplanojamesmulbah$ git branch -m master

oplanos-mbp:gym-git-exercise-solutions oplanojamesmulbah$ git branch
master

oplanos-mbp:gym-git-exercise-solutions oplanojamesmulbah$ git status
On branch master
No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        README.md

nothing added to commit but untracked files present (use "git add" to track)

oplanos-mbp:gym-git-exercise-solutions oplanojamesmulbah$ git add .

oplanos-mbp:gym-git-exercise-solutions oplanojamesmulbah$ git status
On branch master
No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   README.md

oplanos-mbp:gym-git-exercise-solutions oplanojamesmulbah$ git commit -m "
> Initial commit
>
> - Add initial README.md file with project description
- Create table of contents for exercise solutions
- Set up structure for Bundle> - Create table of contents for exercise solutions
> - Set up structure for Bundle 1 with placeholders for exercises
> - Include basic formatting and code blocks for command examples"
[master (root-commit) 0164885] Initial commit
 1 file changed, 23 insertions(+)
 create mode 100644 README.md

oplanos-mbp:gym-git-exercise-solutions oplanojamesmulbah$ git status
On branch master
nothing to commit, working tree clean

oplanos-mbp:gym-git-exercise-solutions oplanojamesmulbah$ git remote add origin https://github.com/mulbahoplanojames/gym-git-exercise-solutions.git

oplanos-mbp:gym-git-exercise-solutions oplanojamesmulbah$ git push
fatal: The current branch master has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin master

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

oplanos-mbp:gym-git-exercise-solutions oplanojamesmulbah$  git push --set-upstream origin master

Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 582 bytes | 582.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/mulbahoplanojames/gym-git-exercise-solutions.git
 * [new branch]      master -> master
branch 'master' set up to track 'origin/master'.

oplanos-mbp:gym-git-exercise-solutions oplanojamesmulbah$ git checkout -b dev
Switched to a new branch 'dev'

oplanos-mbp:gym-git-exercise-solutions oplanojamesmulbah$ git checkout -b test
Switched to a new branch 'test'

oplanos-mbp:gym-git-exercise-solutions oplanojamesmulbah$ git checkout dev
Switched to branch 'dev'

oplanos-mbp:gym-git-exercise-solutions oplanojamesmulbah$ git branch -d test
Deleted branch test (was 0164885).

oplanos-mbp:gym-git-exercise-solutions oplanojamesmulbah$ git push
fatal: The current branch dev has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin dev

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

oplanos-mbp:gym-git-exercise-solutions oplanojamesmulbah$ git push --set-upstream origin dev
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'dev' on GitHub by visiting:
remote:      https://github.com/mulbahoplanojames/gym-git-exercise-solutions/pull/new/dev
remote:
To https://github.com/mulbahoplanojames/gym-git-exercise-solutions.git
 * [new branch]      dev -> dev
branch 'dev' set up to track 'origin/dev'.

oplanos-mbp:gym-git-exercise-solutions oplanojamesmulbah$

```

### Exercise 2

```bash

```
