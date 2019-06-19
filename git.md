1. `git help <command_name>`

2. To set username:

    ```
    git config --global user.name "Gourav Chawla"
    git config --global user.email anything@exampledomain.com
    ```

    1. Check already present usernames: `git config user.name`

    2. Check usernames and email address: `git config --list`

    3. Also, you can view it in the `~/.gitconfig` file
    
> NOTE: The above configurations are for every git project. You can also change them on a project by project basis.

3. Initialize new git repo in current directory
				: `git init`

4. To check status of files in repo (commited, modified etc)
				: `git status`

5. To add files to staging area
				: `git add index.html(file name)`

    1. Add directory to staging area
				: `git add css(directory name)`

6. To commit a file
				: `git commit -m index.html`

7. To show the commit history (How many commits and which commits)
				: `git log`


******************************************************************************

1. To find what changes has been made to a file; Lines added or removed
				: `git diff`

2.  To see changes if file has been staged
				: `git diff --staged`

3. To unstage file
				: `git reset HEAD <filename>`

4. To commit a tracked file(Already staged file, skip staging and commit)
    ```
    git commit -a -m "Modify index.html"
    git commit -am "Modify index.html"
    ```

5. To add files to last commit. Made commit but forgot add a file. So, now to amend commit:
				: `git commit --amend -m "Modify index.html & cats.html"`

6. To undo commit and add back to staging area
				: `git reset --soft HEAD^`

7. Adding a remote
				: `git remote add origin https://github.com/gregg/git-real.git`
    1. Remove Remote: `git remote remove <remote_name>`

8. To push the changes to remote
				: `git push -u origin master  (origin: remote repo name; master: local branch to push)`

******************************************************************************

1. Clone a repo
				: `git clone url <folder_name>`

2. Check the remotes
				: `git remote -v`

3. Create a branch to work on a different feature
				: `git  branch grooming(name of branch)`

4. Switch to branch grooming
				: `git checkout grooming`
				
    1. Checkout and create branch
				: `git checkout -b <branch name>`


5. Merge branch into master
				: `git merge grooming`

6. Clean up the branch/ delete it
				: `git branch -d <branch_name>`



******************************************************************************

### Commands that I came accross

1. Remove files after updated gitignore
        : `git rm -r --cached .`
        
    Before doing this you should commit all the changes that are not commited. 
    Then do `git add .` to add all the files minus the files in gitignore. Commit and you are good to go.

2. Unstage files :
			`git reset filename`

3. Rebase tutorial :
    `https://asciinema.org/a/78683`

4. See log in one line :
    `git log --oneline`

5. Stash ([Problem statement](https://stackoverflow.com/questions/19216411/how-do-i-pull-files-from-remote-without-overwriting-local-files))
    ```
    git stash
    git pull origin master
    git stash pop
    ```

6. Undo rebase ([Reflog & hard reset](https://stackoverflow.com/questions/134882/undoing-a-git-rebase))
