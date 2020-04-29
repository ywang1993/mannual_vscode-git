## Use git in vscode
### Steps:
1. Create a directory on the local file system.
2. Create a repo on Github.
3. Select Clone "Clone or download" on Github, copy the link
4. In Visual Studio Code, sect File -> Add Folder to Workspace -> Select the newly created directory
5. Select Terminal Window
6. In the window, type:
```
git config --global user.name <github userID>
git config --global user.email <email>
git clone <URL from github link copied earlier>
```

That should be all that's required.  any newly created file should be available on github after `stage` / `commit` / `push`.


### Bring local folder to github repo
1. Create a new repository on GitHub.
2. Open Git Bash.
3. Change the current working directory to your local project.
4. Initialize the local directory as a Git repository.
    ```
    $ git init
    ```
5. Add the files in your new local repository. This stages them for the first commit.
    ```
    $ git add .
    ```
6. Commit the files that you've staged in your local repository.
    ```
    $ git commit -m "First commit"
    ```
7. At the top of your GitHub repository's Quick Setup page, click to copy the remote repository URL.
8. In the Command prompt, add the URL for the remote repository where your local repository will be pushed.
    ```
    $ git remote add origin <remote repository URL>
    # Sets the new remote
    $ git remote -v
    # Verifies the new remote URL
    ```
9. Push the changes in your local repository to GitHub.
    ```
    $ git push origin master
    ```