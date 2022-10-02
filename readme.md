# GIT

## What is Git?

    Git is free and open source software for version control, tracking changes in any set of files, usually used for coordinating work among programmers collaboratively developing source code during software developement.

## What is version control?

    Version constrol is a class of systems responsible for managing changes to computer programs, documents, large programs, and so on.

### Types of Version Control System:

    1. Local Version Control Sytems: 
    
        - It is a local database in a local computer, in which every file is saved as a patch. Every patch set contains only the changes made to the file since last version. 

        - The main problem with this is that if any damage happens to the local computer, the whole patch gets lost, further, any damage happens to a single version, the following versions are lost.

    2. Centralized Version Control System:

        - It has a single server that contains all the file verions. It enables multiple clients to pull the file, make changes, and push again to the server. It helps a team to work together on the same file at a server.

        - The main problem with this VCS is that everything is stored on a centralized server, if anything happens to this server, the whole data is lost and cannot be recovered if there is no backup. Hence, it can create chaos in the team.

    3. Distributed Version Control System:

        - With distributed version control systems, clients don’t just check out the latest snapshot of the files from the server, they fully mirror the repository, including its full history. 
        
        - Thus, everyone collaborating on a project owns a local copy of the whole project, i.e. owns their own local database with their own complete history. 
        
        - With this model, if the server becomes unavailable or dies, any of the client repositories can send a copy of the project's version to any other client or back onto the server when it becomes available. It is enough that one client contains a correct copy which can then easily be further distributed.

## `GIT is a well-known example of Distributed Version Control System.`

<hr>
<hr>

## Git Areas

![alt text](https://file%2B.vscode-resource.vscode-cdn.net/var/folders/pv/hyb3d5nx1t7fwpd2d_62xszc0000gn/T/com.apple.Notes/HardLinkURLTemp/A6A7532C-EF7A-470B-919C-C48AB190E721/1664341955/Working.png?version%3D1664672430308)

# Git Tools:

    1. GitBash

        - GitBash is an appilcation for Windows environment. It is used as a git command line for Windows. Bash is an abbreviation of Bourne Again Shell. Git package installer contains Bash, bash utilities, and Git on a Windows operating system.

    2. git gui

    3. gitk

## Basic Command Lines

|PURPOSE|COMMAND|DESCRIPTION|
|:---|:---|:---|                                                                                               
|Print Working Directory|pwd|-Print the location of current working directory|
|Navigate Directories|cd directoryName|- Get in to the directoryName folder
|List all files and folders|ls -la|- Gives a list of all the files and folder within the working directory
|Create new Directory|mkdir directoryName|- Creates new directory
|Create multiple directories at a time|mkdir directory1 directory2|- Creates two directories at a time
|Create new file|touch fileName.txt|- Creates text file named fileName
|Make Changes to the file|nano fileName.txt|- dOpens a pad to make changes to fileName.txt
|Read file|cat fileName.txt|- Content of the file will be displayed to the terminal console
|Copy file|cp fileName.txt file2.txt|- Copy the content of fileName.txt to file2.txt
|Rename File/Folder|mv file1.txt fileOne.txt|- file1.txt will be renamed to fileOne.txt
|Move File to a Folder|mv file.txt folder|- Moves file.txt to folder
|Move multiple files|mv -t backups file1 file2 file3 : For mac: mv file1 file2 ... folder|- Moves file1 file2 file3 to backups folder
|Recursive copy|cp -r backups backup-2|- Copies all the non-empty files and subfolders of backups to backup2
|Delete a file|rm file.txt|- Deletes file.txt
|Delete empty folder|rmdir folder|- Deletes the folder
|Delete non-empty folder|rmdir -rf folder|- Deletes recursively the files and subFolders also

## Git Command Lines

1. Install Git: 
    ```
        install git
    ```
2. Checking status of the repository: 
    ```
        git status
    ```
3. Configure name and email:
    ```
        git config --global user.name 'yourname'
        git config --global user.email 'youremail'
    ```
4. Create a local git repository:
    ```
        mkdir project_name
        cd project_name
    ```
5. Initialize Git:
    ```
        git init
    ```
6. Add file to the staging area : 
    
    For single file
    ```
        git add filename
    ```
    For multiple files
    ```
        git add filename1 filename2
    ```
    To add all files and folders at once
    ```
        git add .
    ```
    To add and commit at the same time
    ```
        git commit -am 'commit message'
    ```
7. Unstage a file
    ```
        git reset HEAD filename
    ```
8. Commit the changes
    ```
        git commit -m 'your message'
    ```
9. Git log
    ```
        git log
    ```
10. List minified log history
    ```
        git log --oneline
    ```
11. List 5 commit history
    ```
        git log --5
    ```
12. Git check out
    ```
        git checkout commit-id
    ```
13. Creating a branch

    Only to create branch
    ```
        git branch  branch-name
    ```
    To create and checkout to the branch at the same time
    ```
        git checkout -b branch-name
    ```
    To switch between branches
    ```
        git checkout main
        git checkout branch-name
    ```
    To list down all the branches
    ```
        git branch
    ```
14. Create account on GitHub

    GitHub Sign up on GitHub

15. Create Repository on GitHub

    Go to GitHub and create a repository by click the plus icon on the top right corner.

16. Connecting git with remote repository
    ```
        git remote add origin remote_repository_ul
    ```
17. Push
    ```
        git push -u origin master
    ```
18. Merge
    ```
        git checkout develop
        git merge feature
    ```
19. Pull
    ```
        git checkout yourbranch
        git pull origin develop 
    ```
    ```
        git checkout develop
        git merge yourbranch
        git push -u origin develop
    ```
20. Git clone
    ```
        cd Desktop
        git clone https://github.com/Asabeneh/10-days-of-git-and-github.git
    ```
21. Rename Branch

    To rename a current branch
    ```
        git branch -m <newname>
    ```
    To rename any branch
    ```
        git branch -m <oldname> <newname>
    ```
22. Deleting Branch

    To delete a local branch
    ```
        git branch -d branch-name
        git branch -D branch-name
    ```
    To delete remote branch
    ```
        git push <remote_name> :<branch_name>
    ```
    or
    ```
        git push <remote_name> --delete <branch_name>
    ```
23. The .gitignore file: 

    To avoid committing those files which one does not want to commit over the git, for example, sensitive information like, passwords, bank account, and so on.
24. Forking:

    A forking is a process of owning other repository. After you clicked on fork button of a certain repository you will see that that repository became in your repository list. You can try by clicking the fork button on this repository.






















        






