# Git Exercises

This comprehensive exercise combines essential Git skills, from manipulating history to advanced branching strategies.

### Resources

Before starting this exercise, Go through **Branching Model** and **Contribution rules and git flow** resources. When attempting the challenges, Try to use what you read as much as you can.

- [Branching Model](https://classic-cobalt-104.notion.site/Branching-model-c1f8f9686eef4d3594a8c1ca4955d451)
- [Contribution rules and git flow](https://classic-cobalt-104.notion.site/Contribution-rules-and-git-flow-0505d789170f4c0a8b7b5d7b41df7bf5)

### Getting Started:

1. **Create a New Git Repository:**

   - Head over to GitHub and create a new repository. Clone this repository to your local machine.

   ```bash


   ```

2. **Initialize Your Environment:**

   - Open a terminal window and navigate to your cloned repository directory.
   - Run the following commands to create some dummy files and commit them:

   ```bash
   touch test{1..4}.md
   git add test1.md && git commit -m "chore: Create initial file"
   git add test2.md && git commit -m "chore: Create another file"
   git add test3.md && git commit -m "chore: Create third and fourth files"
   ```

## Challenges:

**Part 1: Refining Git History (10 Challenges)**

1. **Missing File Fix:**

   - Run `git status` and `git log` to assess the current state of your repository.
   - From the status you will see that you forgot to add `test4.md` in the last commit.

   **Challenge:** Recover from this error by staging/adding `test4.md` and amending the commit message with an appropriate description.

```bash
Rich.com@DESKTOP-3TOVTRS MINGW64 ~/Documents/Things/The Gym/Git/advanced-git (main)
$ git status
On branch main
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        test4.md

nothing added to commit but untracked files present (use "git add" to track)

Rich.com@DESKTOP-3TOVTRS MINGW64 ~/Documents/Things/The Gym/Git/advanced-git (main)
$ git log
commit 8fae7631f217911a02944d0c779ad4ac70733c2a (HEAD -> main)
Author: MikeManzi <manzimike378@gmail.com>
Date:   Tue May 21 12:25:58 2024 +0200

    chore: Create third and fourth files

commit b291a72408e1930e43124c031c5e25e0b9338e0d
Author: MikeManzi <manzimike378@gmail.com>
Date:   Tue May 21 12:25:57 2024 +0200

    chore: Create another file

commit 1438792869560a2da326bacbdab0e933984f2789
Author: MikeManzi <manzimike378@gmail.com>
Date:   Tue May 21 12:25:57 2024 +0200

    chore: Create initial file

Rich.com@DESKTOP-3TOVTRS MINGW64 ~/Documents/Things/The Gym/Git/advanced-git (main)
$ git add test4.md

Rich.com@DESKTOP-3TOVTRS MINGW64 ~/Documents/Things/The Gym/Git/advanced-git (main)
$ git commit --amend --no-edit
[main de09fdb] chore: Create third and fourth files
 Date: Tue May 21 12:25:58 2024 +0200
 2 files changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 test3.md
 create mode 100644 test4.md
```
