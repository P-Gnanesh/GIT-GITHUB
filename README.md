# GIT & GITHUB
---------------------------------------------------------------------------------------------------------------------------
This is a simple repo that is used for understanding the basics of git and github.
Git is a version control system that is mainly used to track,maintain,control and save the changes that are made in the source code in the application development
Github is a website that is mainly used to store the git managed repositories using git.


GitHub provides features like code sharing , pull requests , collaboration.

1) Git --version -> For checking out the current git version available in your local system.

2) Git clone -> Cloning is mainly used for copying the files of the required repository to the local system [Syntax: git clone (Link of the repo)]

3) Redirecting the current directory to the actual project file(DemoSetup) not the project folder (GITHUB_FOLDER) [Syntax: cd DemoSetup]

4) Git status -> This command is used to show the current status of the changes made in the local system [Syntax: git status]

5) Git Status is divided into 4 categories:
   i) Untracked Status - It means that the new files are created but they are not recognized or tracked by the git.
   ii)Modified Status - It refers to the changes or modification made to the existing files.
   iii)Unmodified Status - It refers to no modification or the changes 
   iv)Staged Status - It refers that the files are tracked by the git but not yet committed(ready to commit)

   [Note: When new files are created , these files are not automatically tracked by the gitwhich is why we get the status as "Untracked".In order to make these files tracked by git we use git add command]

6) Git Add -> This command is mainly used for the files to be tracked by the Git in your local system.It can be written in 3 ways.
  i) [Syntax1: git add file_name] ->Only individual files are tracked by the git
  ii) [Syntax2: git add .] -> Tracks all the files in the project instead of a single file
  iii) [Syntax3: git add -v]

7) Git Commit -> By using git commit we make sure that we store and save all these changes in a single commit (like on 26-6-26 I added index and login file on a daily basis )[Syntax: git commit -m "mssg"]

8) Git Push -> After commiting the files we can push these files to our GitHub account[Syntax: git push]

--------------------------------------------------------------------------------------------------------------------------

Most of the  people assume git and github to be same but both are different.Git is a version control system software that is mainly used to track ,manage ,save  and to control the changes made in the source code during the development of the software.Git holds the history of the code.

For example, I create  a project  all alone by myself which is being stored in my local system like laptop, so as the project grows , its complexity  would  also grow which leads to the difficulty in manually  managing the code changes so we need a software that saves each stage of the project like if at one stage of implementation my project crashes so we must have a software to revert back to the previous version of the project and rewrite the code ,this can be done by git.

The project is saved in the developers local system but it cannot be  accessed by other developers .In order to make the project publicly available we need a cloud platform. GitHub is such a platform that is mainly used for storing the git managed projects so that others can access and modify it.

Let's  consider a scenario where a project is being built by multiple developers, each individual developer builds his part of the application in his local system. But a project can be only be created if all the individual appliactaion parts of the developers get combined, that can be done  with the help of github.

Initially in GitHub we create a project folder called a repository where the project code from multiple developers can be pushed to this folder. All the code together will form a complete project.

----------------------------------------------------------------------------------------------------------------------------

**How developers share code:**

**Scenario 1 - Developers are a part of the official team (Contributors)** -> Consider a project is being built by multiple developers. Let's Consider two Developers "A" and "B".

Imagine Devloper A creates a new repository in his github account for a project. The repository still lies in the local system of the Developer A so even though the repo is created the other teammates(B) cannot access it. So the Developer A needs to send a invite to Developer B in order to  become a Collaborator.He now will be provided with the "write access" through which he can add and edit the files.Developer B doesnt have to fork.He then clones the project files to his local system and can make the changes.Developer B can then push back all the newly added files back to the original github account.


Here is the exact lifecycle of how a team member modifies the project:

Step 1: Clone (Downloading the Project)
A developer on your team doesn't just download a ZIP file. They use Git to Clone the repository.

What it does: This downloads the entire history of the project, all its versions, and all its branches from the GitHub cloud onto their local laptop. Now, their local system has a perfect mirror of the GitHub repository.

Step 2: Local Editing & Tracking
The developer writes code on their laptop.

They might add a new feature or fix a bug.

As they work, they make local Commits (those video game checkpoints we talked about). At this stage, these changes only exist on their laptop. The central GitHub repository remains untouched, and other teammates cannot see this work yet.

Step 3: Pushing the Code
Once the feature is fully built, tested, and working locally, the developer runs a Git command to Push their local commits up to the main-project repository on GitHub.

Step 4: Updating the Team
Because the central GitHub repository now has the new code, the other developers on the team run a Git command to Pull the latest changes. This downloads the updates onto their respective laptops, ensuring the whole team is perfectly synced.

---------------------------------------------------------------------------------------------------------------------------

**Scenario 2 - Developers are an outside stranger (Open Source)** -> Consider the same developers "A" and "B" working individually. 

Developer A creates a repository for his project and pushes it back to the github rep. Developer B(outsider) cannot access the original repo of A. So he must fork(creating a duplicate copy of the repository) the github repo of the developer A into his own github account. He then can clone all the files to his local system and can make all the chnages required.He can then push the newly added and edited files back to his github account but not to the Developer A's account. For changing the 
Developer A's code the Developer B needs to pull a request to the Developer A via Pull Request button in the github account.
The Developer A can then compare , checks for conflicts,can give feedback and thn can merge the code einto his repository.

Here is the exact lifecycle of how a outsider can  modify the project:

Step 1: Forking (Creating a Personal Copy)
The outside developer goes to your GitHub page and clicks the "Fork" button.

What it does: GitHub instantly duplicates your entire repository and puts that copy into their personal GitHub account (e.g., stranger-username/main-project).

Because this copy belongs to them, they have full control and permission to modify it.

Step 2: Clone & Local Work
Just like the team member, the stranger clones their own forked version down to their local laptop, makes the necessary code changes, and saves their progress using local Git commits.

Step 3: Pushing to Their Own Fork
The stranger pushes these new commits from their laptop back up to their own GitHub account. Your original repository still hasn't changed at all.

Step 4: The Pull Request (The Suggestion Box)
To give the fix back to you, the stranger goes to GitHub and opens a Pull Request (PR).

A Pull Request is essentially a formal message that says: "Hey Sandeep, I noticed a bug in your project and fixed it in my copy. Here are the exact lines of code I changed. Please review it, and if you like it, click 'Merge' to pull these changes into your original project."

Step 5: Review and Merge
As the project owner, you get a notification. GitHub shows you a clean, side-by-side comparison of your original code versus their modified code.

If their code is good, you click "Merge". GitHub automatically grabs their changes and blends them into your original project.

If their code has issues, you can comment on the lines of code, chat with them, and ask them to fix it before you accept it.

----------------------------------------------------------------------------------------------------------------------------

**Confused between Clone and Fork 😕🤔**

FORK = Cloud-to-Cloud Copy. You make a copy of someone else's book on GitHub and put it on our GitHub account. It is still in the cloud.

CLONE = Cloud-to-Laptop Copy. We download a copy of a book from GitHub onto our actual physical computer so we can type on it.

----------------------------------------------------------------------------------------------------------------------------

**Commit**

By committing we can tell the git to save all the changes made in a single commit.

WE use Commit when we are actively writing code on our laptop and saving our incremental progress. A commit represents a micro-checkpoint.

Frequency: Multiple times a day (sometimes every 15–30 minutes).

When to use it: Every time you finish a small, isolated task or fix a specific thing.
Examples of when you create a commit:You fixed a typo on the homepage. $\rightarrow$ Commit
       You finished writing the logic for the password reset button. $\rightarrow$ Commit
       You changed the background color from blue to grey. $\rightarrow$ Commit

----------------------------------------------------------------------------------------------------------------------------

**Version**

A pack of commits can be called as a version.

We use Version (also called a "Release" or a "Tag") when we bundle a massive group of individual commits together to mark a major, stable milestone of the application that is ready for the public or the user.
Frequency: Infrequently (weeks or months apart).

When to use it: When the software reaches a complete, fully tested state that people can actually use.
Examples of when you label a version:The entire application is built and ready for launch. $\rightarrow$ Version 1.0.0
You added 50 new features and fixed 20 bugs over the last month. $\rightarrow$ Version 2.0.0

----------------------------------------------------------------------------------------------------------------------------


**🛠️ Git Commands & Workflow**

**Scenario 1: Command Workflow for using an existing repository from github**

1) **git --version** -> Displays the exact version of Git installed on our local system. We can run this command in our computer's native Terminal or directly inside the VS Code integrated Terminal.

2) **git clone <repository_link>** -> This is our first step when working with an existing project. Cloning copies the entire remote repository hosted on GitHub down to our local machine.We can copy this URL by clicking the green "Code" button on our GitHub repository page.

3) **git status** -> This command displays the state of the working directory and the staging area. It lets us to see which changes have been staged, which haven't, and which files aren't being tracked by Git yet.

The Correct Terminal Sequence:

   **Bashgit --version**               
   **git clone <repository_link>**     
   **cd directory**                    
   **git status**                      


🚦 File Lifecycles & States -> When we run git status, files are categorized into distinct tracking states:

1)Untracked: Brand new files created locally that Git is not yet watching.
2)Modified: Existing files that have been changed or edited.
3)Unmodified: Files that have no new changes compared to the last save point.
4)Staged: Tracked changes that are prepared and bundled, ready to be officially saved in the next commit snapshot.
   
Moving from Untracked to Tracked -> New files do not get saved by Git automatically. To move files into the Staged area, we must manually run the **git add** command. 
Once staged, we use **git commit** to seal them into our project's official history timeline.


4) **📥 Git Add:** 
Three Methods:
**git add <file_name>** $\rightarrow$ Stages a single, specific file.
**git add .** $\rightarrow$ Stages every single modified and untracked file in your current folder all at once.
**git add . -v** $\rightarrow$ Stages all files and prints an explicit confirmation message in the terminal for every file tracked.

5) **🔒 Git Commit:**
**Bashgit commit -m "Brief description of changes made"**

git add organizes your files into a temporary staging bundle.
git commit takes that bundle and creates a permanent, encrypted snapshot in our local repository timeline.
We must do this routinely to document oour daily coding progress.

6) **🚀 Git Push**: 
Once our local snapshots are committed,we can send them up to the cloud: **Bashgit push**
Because we cloned this repository directly from GitHub, our local system already tracks the remote destination automatically. Running git push updates our cloud profile instantly.

----------------------------------------------------------------------------------------------------------------------------

**Scenario 2 : Linking a Local Project Folder to github repository**

Unlike the previous scenario where the developer uses an existing project and clones it to his local system , make changes and push it back to his github repo the scenario 2 is mainly about understanding the process and the commands used to upload a local project folder to his github account.

Intially consider a Developer who is making a project using any of the text editors in his local system. Usually the github repository can only be linked to a git folder which is being tracked by the git and not by any local folder. So , for this the developer needs to first convert the local folder to a git folder using the command **git init** . Init command is mainly used to convert an existing local folder in the local system to a git folder.Now this folder is being tracked by git.

The developer then can create a repo in his github account.
[Note: It is recommended not to even enable a readme file in the github while creating a repo.Instead create a one in ur local system. ]
The developer has  converted the local folder to a git folder but the folder is not yet  linked to the github repo.
For connecting or linking the git projrct folder  to the particular github repo we need to use a command
**git remote add origin <"Link of the repo">**

Now all the changes developer make in his local system will be done will be linked to the repo.

**git remote -v** This command is mainly used to check whether the connected repository is correct or not.

----------------------------------------------------------------------------------------------------------------------------

Git Branch

What is a Branch?
A branch is a separate line of development inside a Git repository.
It allows developers to work on new features or changes without affecting the main/stable code.
Example:
You have a project:

main branch
A ---- B ---- C

Here:

main contains the stable version of the project
Every commit represents a saved version

Now you want to add a login feature.

Instead of changing main directly, create a new branch:

              login-feature
                    |
A ---- B ---- C ---- D ---- E
                    |
                  main

Now:

main → original stable code
login-feature → development code

After completing the feature, it can be merged back into main.

2. Check Current Branch:[Syntax ->**git branch**]
Explanation: Displays all branches available in the repository.
Example output:
* main
  login-feature

Meaning: * indicates the branch you are currently working on
Current branch = main

3. Create a New Branch: [Syntax->**git branch  branch_name**

Example: git branch  login
Explanation: Creates a new branch called login.

Before:

main
A ---- B ---- C

After:

              login
                |
A ---- B ---- C
                |
              main

[Important: Creating a branch does not move you into that branch.You are still on main.]

4. Switch to a Branch:[Syntax->**git checkout branch_name**]

Example: git checkout login

Explanation: Moves your working area from one branch to another.

Before:
* main
  login

After:
  main
* login

Now all changes you make will happen inside login branch.

5. Create and Switch Branch Together:[Syntax->**git checkout -b branch_name**]

Example: git checkout -b payment

Explanation
This performs two actions:

Creates a new branch
Automatically switches to it

Instead of:
git branch payment
git checkout payment

You can do both together:
git checkout -b payment


6. Rename a Branch: [Syntax-> **git branch -m new_branch_name**]

Example:
git branch -m development
Explanation

Changes the name of the current branch.

Example:
Before:
master

After:
development


7. Delete a Branch:[**Syntax->  git branch -d branch_name**]

Example:
git branch -d login

Explanation
Deletes a branch after its work is completed.

Example:
main
 |
 |
merged login feature
 |
delete login branch

The code remains in main after merging.

----------------------------------------------------------------------------------------------------------------------------

!) Merge Branches

What is Merge?
Merge is used to combine changes from one branch into another branch.

Example:

Main:

main

A ---- B ---- C

Feature branch:

login

A ---- B ---- C ---- D ---- E

Now login feature is complete.

Move to main:
git checkout main

Merge:
git merge login

Result:

A ---- B ---- C ---- D ---- E
                    |
                  main

Now main contains login changes.

2) Automatic Merge: Git performs automatic merge when it can combine changes without confusion.
Example:

Main branch:
System.out.println("Hello");

Feature branch:
System.out.println("Welcome");

If changes are in different places:

file1.java  → changed by main
file2.java  → changed by feature

Git understands and merges automatically.
No manual work needed.

3) Merge Conflict
What is Merge Conflict?
A merge conflict occurs when Git cannot decide which change to keep.

Example:
Main branch:
System.out.println("Hello");

Feature branch:
System.out.println("Hi");

Both modified the same line.

Git gets confused:

Which one should I keep?
Hello or Hi?

So Git marks:

<<<<<<< HEAD

Hello
=======
Hi

<<<<<<< login

Resolving Merge Conflict

You manually edit the file.

Example:
Keep:
System.out.println("Hello Hi");
Then tell Git:

Step 1
git add .
Meaning: "Conflict is solved, prepare this file."

Step 2
git commit -m "Resolved merge conflict"

Meaning: Save the conflict resolution.










