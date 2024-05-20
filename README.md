# Git tutorial for work 
- 1. Go to folder where you want to create repository
- 2. In cmd or git bash run command:
git init
- 3. Command:
git status
Will show that commits and files that have been tracked earlier

files can be in **2** states
`Tracked` - files that Git knows about and are added to repository
`Untracked` - files that Git don\`t knows about and don\`t be added to repository

- 3. 1) For tracking :green_book: files you could use this command: 
```
git add <file>
```
- 3. 2) For untracking :closed_book: previously tracked file(s) you could use this command:
```
git rm --chached <file>
```
Staging Env - its environment that have info about all tracking files

- 3. 3) This command will tracking :green_book: all files that you add:
```
git add --all 
or
git add -A
```
- 3. 4) If file was **modified** we could restore them from **Staging env** by using this command:
```
git restore --staged <file>
```
- 4. Adding commits keep track of our progress and changes as we work. Git considers each commit change point or "save point". It is a point in the project you can go back to if you find a bug, or want to make a change.
```
git commit -m "First release of git_tutorial!"
[master (root-commit) 221ec6e] First release of Hello World!
 3 files changed, 26 insertions(+)
 create mode 100644 README.md
 create mode 100644 bluestyle.css
 create mode 100644 index.html
```

The commit command performs a commit, and the -m "message" adds a message.

The Staging Environment has been committed to our repo, with the message:
"First release of git_tutorial!"
- 4. 1) If we have small changes in some files we could commit with flag **-a**:
```
git commit -a -m "First release of git_tutorial!"
```
answer
```
[master 09f4acd] Updated index.html with a new line
 1 file changed, 1 insertion(+)
```
- 4. 2) For checking **git status** :ledger: in more good visible form we could use this command:
`
**Note:** Short status flags are:

    ?? - Untracked files
    A - Files added to stage
    M - Modified files
    D - Deleted files
`
- 4. 3) For checking history of commits you could use this command :book: :
```
git log
```
- 5. If you are having trouble remembering commands or options for commands, you can use Git help.

There are a couple of different ways you can use the help command in command line:

- 5. 1) `git command -help` -  See all the available options for the specific command
- 5. 2) `git help --all` -  See all possible commands
 Let's go over the different commands.

- 6. We are working in our local repository, and we do not want to disturb or possibly wreck the main project.

So we create a new branch with command:
```
git branch <name of branch>
```
