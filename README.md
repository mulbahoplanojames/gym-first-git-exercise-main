# Gym Git Exercise Solutions

This README file contains my solutions for most of the bundles of the Git exercises provided to us by our coaches, in person of Tresor Manzi and Souvede Inshuti from the gym.

## Table of Contents

- [Bundle 1](#bundle-1)
  - [Exercise 1](#exercise-1)
  - [Exercise 2](#exercise-2)

## Bundle 1

### Exercise 1

```bash
# Initialized a new Git repository
oplanos-mbp:gym-git-exercise-solutions oplanojamesmulbah$ git init
Initialized empty Git repository in /Users/oplanojamesmulbah/gym-git-exercise-solutions/.git/

# Check status after initialization
oplanos-mbp:gym-git-exercise-solutions oplanojamesmulbah$ git status
On branch main
No commits yet
nothing to commit (create/copy files and use "git add" to track)

# Rename main branch to master
oplanos-mbp:gym-git-exercise-solutions oplanojamesmulbah$ git branch -m master

# Verify branch name change
oplanos-mbp:gym-git-exercise-solutions oplanojamesmulbah$ git branch
* master

# Check status
oplanos-mbp:gym-git-exercise-solutions oplanojamesmulbah$ git status
On branch master
No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        README.md

nothing added to commit but untracked files present (use "git add" to track)

# Add README.md file
oplanos-mbp:gym-git-exercise-solutions oplanojamesmulbah$ git add .

# Check status
oplanos-mbp:gym-git-exercise-solutions oplanojamesmulbah$ git status
On branch master
No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   README.md

# Commit changes
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

# Check status
oplanos-mbp:gym-git-exercise-solutions oplanojamesmulbah$ git status
On branch master
nothing to commit, working tree clean

# Add remote repository
oplanos-mbp:gym-git-exercise-solutions oplanojamesmulbah$ git remote add origin https://github.com/mulbahoplanojames/gym-git-exercise-solutions.git

# Push changes
oplanos-mbp:gym-git-exercise-solutions oplanojamesmulbah$ git push
fatal: The current branch master has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin master

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

# Push changes
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

# Create and switch to the dev branch
planos-mbp:gym-git-exercise-solutions oplanojamesmulbah$ git checkout -b dev
Switched to a new branch 'dev'

# Create and switch to the test branch
planos-mbp:gym-git-exercise-solutions oplanojamesmulbah$ git checkout -b test
Switched to a new branch 'test'

# Switch to the dev branch
oplanos-mbp:gym-git-exercise-solutions oplanojamesmulbah$ git checkout dev
Switched to branch 'dev'

# Delete the test branch
oplanos-mbp:gym-git-exercise-solutions oplanojamesmulbah$ git branch -d test
Deleted branch test (was 0164885).

# Push changes
oplanos-mbp:gym-git-exercise-solutions oplanojamesmulbah$ git push
fatal: The current branch dev has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin dev

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

# Push dev branch to remote
oplanos-mbp:gym-git-exercise-solutions oplanojamesmulbah$ git push --set-upstream origin dev
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'dev' on GitHub by visiting:
remote:      https://github.com/mulbahoplanojames/gym-git-exercise-solutions/pull/new/dev
remote:
To https://github.com/mulbahoplanojames/gym-git-exercise-solutions.git
 * [new branch]      dev -> dev
branch 'dev' set up to track 'origin/dev'.
```

### Exercise 2

```bash

# Created home.html and tried to stash (no changes to stash)
oplanos-mbp:gym-git-exercise-solutions oplanojamesmulbah$ touch home.html
oplanos-mbp:gym-git-exercise-solutions oplanojamesmulbah$ git stash
No local changes to save

# Checked status
oplanos-mbp:gym-git-exercise-solutions oplanojamesmulbah$ git status
On branch dev
Your branch is up to date with 'origin/dev'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        home.html

nothing added to commit but untracked files present (use "git add" to track)

# Added home.html
oplanos-mbp:gym-git-exercise-solutions oplanojamesmulbah$ git add .
oplanos-mbp:gym-git-exercise-solutions oplanojamesmulbah$ git status
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   home.html

# Stashed home.html
oplanos-mbp:gym-git-exercise-solutions oplanojamesmulbah$ git stash
Saved working directory and index state WIP on dev: 75950fa Add Git exercise 1 solution - Include terminal output for each command in Exercise 1

# Created and add about.html
oplanos-mbp:gym-git-exercise-solutions oplanojamesmulbah$ touch about.html
oplanos-mbp:gym-git-exercise-solutions oplanojamesmulbah$ git add about.html

# Stashed about.html
oplanos-mbp:gym-git-exercise-solutions oplanojamesmulbah$ git stash
Saved working directory and index state WIP on dev: 75950fa Add Git exercise 1 solution - Include terminal output for each command in Exercise 1

# Created and added team.html
oplanos-mbp:gym-git-exercise-solutions oplanojamesmulbah$ touch team.html
oplanos-mbp:gym-git-exercise-solutions oplanojamesmulbah$ git add team.html

# Stashed team.html
oplanos-mbp:gym-git-exercise-solutions oplanojamesmulbah$ git stash
Saved working directory and index state WIP on dev: 75950fa Add Git exercise 1 solution - Include terminal output for each command in Exercise 1

# Applied stashed to home.html
oplanos-mbp:gym-git-exercise-solutions oplanojamesmulbah$ git stash pop stash@{1}
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

# Added about.html
oplanos-mbp:gym-git-exercise-solutions oplanojamesmulbah$ git stash pop stash@{1}
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   home.html

Dropped stash@{1} (ccb8ba0c802331cb7aef304253bdcb10196f737a)

# Add home.html and about.html
oplanos-mbp:gym-git-exercise-solutions oplanojamesmulbah$ git add .
oplanos-mbp:gym-git-exercise-solutions oplanojamesmulbah$ git commit -m "Add and Setup home.hmtl and about.html page"
[dev a88c929] Add and Setup home.hmtl and about.html page
 2 files changed, 24 insertions(+)
 create mode 100644 about.html
 create mode 100644 home.html

# Applied remaining stash with team.html
oplanos-mbp:gym-git-exercise-solutions oplanojamesmulbah$ git stash pop
On branch dev
Your branch is ahead of 'origin/dev' by 1 commit.
  (use "git push" to publish your local commits)

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

Dropped refs/stash@{0} (9c8c9a9db68a33fc0bd1cb223a1188e053da2cb2)

# Reset to previous commit
oplanos-mbp:gym-git-exercise-solutions oplanojamesmulbah$ git reset --hard
HEAD is now at a88c929 Add and Setup home.hmtl and about.html page
```

<!--
git commit -m "Add Git exercise 2 solution

- Include terminal output for each command in Exercise 2 -->
