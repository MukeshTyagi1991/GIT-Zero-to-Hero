1.What is GIT:- Gloabl Information Tracker and also called source code management (SCM)

GIT is a version control system which is used as a source code manager which tarck history of the code .


2.Install the GIT in your system :-

(i).Download git bash for window 

    Git bash ------Linux simulation or Git Bash is a command-line interface (CLI) application for Windows that provides an emulation of a Unix-like Bash shell environment (Git , SSH) 

(ii) Always create a git folder so that your git always track that particlaur folder not all folder for your computer 

Problem with Linix file system
1.can't restore files
2.can't managed version
3.can't understand who edit
4.Can't check edit time

S0 with the help of git we can slove this problem:-

go to the folder:-

1.git init
2.ls -a
3.we need to check file is under git (VCM) or not through git status command 
4.Untracked (git status) -------staged ( git add----tracked or untracked (git rm --chached ) -------tracked (git commit) ----git restore

<img width="1029" height="761" alt="image" src="https://github.com/user-attachments/assets/060b5de4-c251-44cb-94d2-66266beba984" />


Git Commands
1. Initialization
Create a new Git repository:

git init

2. Configuration
Set global username:

git config --global user.name "mukesh"

Set global email:

git config --global user.email "mukeshtyagi017@gmail.com"

3. File Operations
Create a new file:

touch <filename>

Remove a file:

rm <filename>

Restore a deleted file:

git restore <filename>

4. Staging and Commit
Check the status of the repository:

git status

Add a file to the staging area:

git add <filename>

Commit changes with a message:

git commit -m "your commit message"

5. Branching
Create a new branch:

git checkout (switch) -b <branch_name>

Switch between branches:

git checkout <branch_name>

List all branches:

git branch

6. Logs
View commit history:

git log

View concise commit history:

git log --oneline

7. Remove from Staging
Unstage a file (remove from index but keep in working directory):

git rm --cached <filename>

8. Miscellaneous
View all files, including hidden ones:

ls -a

Clear terminal screen:

clear

View command history:

history

git status (all the commit message and log comes from master barch to your dev barch )
<img width="1043" height="571" alt="image" src="https://github.com/user-attachments/assets/993b795d-941e-43a6-a519-ceed21e3c324" />

<img width="509" height="364" alt="image" src="https://github.com/user-attachments/assets/ac8cf057-e4f0-4225-a013-12c1024c9e22" />


