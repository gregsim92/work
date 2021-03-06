$ this one is correct

### Essential Git Commands

####Create a new git repository
`$ git init` - Create a new, local repository

#### Repo Status
`$ git status` - Check the status of your current repository and see which files have changed.

`$ git diff` - Show differences between your working directory and the index.

#### Repo History
`$ git log` - The command takes options applicable to the git rev-list command to control what is shown and how, and options applicable to the git diff-* commands to control how the changes each commit introduces are shown. 

`$ git log --oneline --decorate --color --graph --all` - __Fill Me Out__

`$ git log -p [filename]` If you want to see the actual changes introduced by each commit, you can pass the -p option to git log. This outputs the entire patch representing that commit

#### Stage files to commit
`$ git add <filename>` - he git add command adds a change in the working directory to the staging area. It tells Git that you want to include updates to a particular file in the next commit. However, git add doesn't really affect the repository in any significant way—changes are not actually recorded until you run git commit.

`$ git add -A` - git add -A is equivalent to  git add .; git add -u
git add -u looks at all the already tracked files and stages the changes to those files if they are different or if they have been removed. It does not add any new files, it only stages changes to already tracked files.

#### Commit changes in staged files
`$ git commit -m "<commit message>"` - commits the added/awaiting changes to a file/repository

#### Branching
`$ git branch <branch name>` - Creates a new branch, it does not check the new branch.

`$ git branch` - git branch lists all the branches in a repository

`$ git checkout <branch name>` - returns the master branch. It may be followed by commit to add changes to master branch. 'git revert' or 'git reset' will undo changes made.

#### Merging

`$ git merge <branch name>` - allows you to take individual lines of development and merge them into a current branch. The current branch will be updated, but the target branch will be unaffected. Often used with git checkout for selecting the current branch.
Once you've saved that file, try this:



### Alias
To simplify a command you can use 
"git config--global alias.<shortened command> <command name>
ex: "git config--global alias.st status"