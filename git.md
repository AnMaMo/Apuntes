# GIT Commands and Actions

Create Repo
-----------
|                     |                           |
| ------------------- | ------------------------- |
|**New Local Repo**   | `git init [project-name]` |
|**Copy Remote Repo** | `git clone [url] [?name]` |

Making Changes
--------------
|                                 |                                             |
| ------------------------------- | ------------------------------------------- |
| **Show Changes <short>**        | `git status <-s>`                           |
| **Stage Changes**               | `git add [file]` or `git add .`             |
| **Commit Staged Changes**       | `git commit -m [message]`                   |
| **Amend Previous Commit**       | `git commit --amend`                        |
| **Diff b/w Working and Staged** | `git diff`                                  |
| **Diff b/w Staged and HEAD**    | `git diff --staged` or `git diff --cached`  |
| **Diff b/w Working and HEAD**   | `git diff HEAD`                             |
| **Unstage Changes to File**     | `git reset HEAD [file]`                     |
| **Discard Changes**             | `git checkout -- [file]`                    |

Remote
------
|                        |                                                |
| ---------------------- | ---------------------------------------------- |
| **List Remotes**       | `git remote`                                   |
| **Show Remote Detail** | `git remote show [name]`                       |
| **Add Remote**         | `git remote add [name] [url]`                  |
| **Rename Remote**      | `git remote rename [original-name] [new-name]` |
| **Delete Remote**      | `git remote rm [name]`                         |
| **Push to Remote**     | `git push [remote] [branch]`                   |

Branches
--------
|                                      |                                 |
| ------------------------------------ | ------------------------------- |
| **List Branches**                    | `git branch`                    |
| **Create Branch**                    | `git branch [branch-name]`      |
| **Switch to Branch**                 | `git checkout [branch-name]`    |
| **Merge Branch into current branch** | `git merge [ branch ]`          |
| **Merge Branch1 into Branch2**       | `git merge [branch1] [branch2]` |
| **Delete Branch**                    | `git branch -d [branch-name]`   |