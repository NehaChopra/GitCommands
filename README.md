# Gitty Git
Collection of Git Commands

## <a name='git'>Creating GIT Projects</a>
|               Command                           |                             Explanation                   |
| ------------------------------------------------| ----------------------------------------------------------|
| git init                                        | Initialize git project                                    |
| git clone                                       | Clone git repository from Remote to local                 |

## <a name='snapshot'>Snapshot, Staged, Working Directory</a>
|               Command                           |                             Explanation                   |
| ------------------------------------------------| ----------------------------------------------------------|
| git status                                      | Staging area changes                                      |
| git add [file-name]                             | Add a file to the staging area                            |
| git add -A OR git add .                         | Add all newly added and changed files to the staging area |
| git commit -m "[commit message]"                | Commit changes to working directory                       |
| git rm -r [file-name]                           | Remove a file                                             |
| git commit --amend                              | Ammend a commit                                           |

## <a name='branching'>Branching</a>
|               Command                           |                             Explanation                   |
| ------------------------------------------------| ----------------------------------------------------------|
| git branch                                      | List branches                                             |
| git branch -a                                   | List all branches (local and remote)                      |
| git branch [branch-name]                        | Create a new branch                                       |
| git branch -d [branch-name]                     | Delete a local branch                                     |
| git push origin --delete [branch-name]          | Delete a remote branch                                    |
| git checkout -b [branch-name]                   | Create a new branch and switch to it                      |
| git checkout -b [branch name] origin/[branch-name]| Clone a remote branch and switch to it                  |
| git checkout [branch-name]                      | Switch to a branch                                        |
| git checkout -                                  | Switch to the branch last checked out                     |

## <a name='mergiing&rebasing'>Merging and Rebasing</a>
|               Command                           |                             Explanation                   |
| ------------------------------------------------| ----------------------------------------------------------|
| git checkout -- [file-name]                     | Discard changes to a file                                 |
| git checkout .                                  | Discard all the changes                                   |
| git merge [branch-name]                         | Merge a branch into the active branch                     |
| git merge [source] [target]                     | Clone git repository from Remote to local                 |
| git stash                                       | Stash changes in a staging area                           |
| git stash clear                                 | Remove all stashed entries                                |
| git stash list                                  | List all stashed entries                                  |
| git stash show                                  | File changes in latest stashed entries                    |
| git stash pop                                   | Pop stashed changes                                       |
| git stash apply                                 | Apply changes back to staging area                        |

## <a name='logging'>Logging</a>
|               Command                           |                             Explanation                   |
| ------------------------------------------------| ----------------------------------------------------------|
| git log                                         | Information of previous committed commits                 |
| git reflog show                                 | Commits with hash, heads and messages                     |
| git log --summary                               | Detailed Information of previous committed commits        |
| git log --date-order --all                      | Ordered previous committed commits                        |
| git log --all                                   | All previous committed commits                            |
| git log -3                                      | Last 3 previous committed commits                         |
| git log --author <name>                         | Previous committed commits by author                      |
| git log --committer <name>                      | Previous committed commits by committer                   |
| git log --after "2019-02-01" --before "2019-02-02"| Date range for committed commits                        |
| git log -p                                      | Commits with file diff changes                            |
| git log --stat                                  | Commits with files changes                                | 
| git log --graph                                 | Graph representation of commits                           |   

## <a name='pull&push'>Pull and Push</a>
|               Command                           |                             Explanation                   |
| ------------------------------------------------| ----------------------------------------------------------|
| git push origin [branch-name]                   | Push a branch to remote repository                        |
| git push -u origin [branch-name]                | Push changes to remote repository and remember the branch |
| git push                                        | Push changes to remote repository in remembered branch    |
| git push origin --delete [branch-name]          | Delete a remote branch                                    |
| git pull                                        | Update local repository                                   |
| git pull origin [branch-name]                   | Pull changes for a branch                         |
| git remote add origin ssh://git@github.com/[username]/[repository-name].git| Add a remote repository        |
| git remote set-url origin ssh://git@github.com/[username]/[repository-name].git| Set a repository's origin branch to SSH   |
| git push -f origin [branch-name]                | Force push to a branch, update commit history             |
| git fetch                                       | Fetch the remote branches                                 |

  
## <a name='resetting'>Resetting commits</a>
|               Command                           |                             Explanation                   |
| ------------------------------------------------| ----------------------------------------------------------|
| git reset HEAD~noOfCommits                      | Reset no of commits from head to reset changes            |
| git rebase -i HEAD~noOfCommits                  | Squash a commit to a number                               |
| git checkout <commitHash>                       | Detached head, move to a commit                           |

## <a name='config'>Config Changes</a>
|               Command                           |                             Explanation                   |
| ------------------------------------------------| ----------------------------------------------------------|
| git config --global username "your username"    | Updating .gitConfig with username                         |
| git config --global password "your password"    | Updating .gitConfig with password                         |

## <a name='alias'>Alias</a>
|               Command                           |                             Explanation                   |
| ------------------------------------------------| ----------------------------------------------------------|
| git config --global alias.ph 'push'             |                                                           |
| git config --global alias.pl 'pull              |                                                           |
| git config --global alias.st 'status -sb'       |                                                           |
| git config --global alias.cm 'commit -m'        |                                                           |
| git config --global alias.rv 'remote -v'        |                                                           |
| git config --global alias.d 'diff'              |                                                           |
| git config --global alias.co checkout           |                                                           |
| git config --global alias.br branch             |                                                           |
| git config --global alias.ci commit             |                                                           |  
|git config --global alias.gl 'config --global -l'|                                                           |  

  


Worth Reading : https://opensource.com/article/20/11/git-aliases
