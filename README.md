# GIT & GITHUB
This is a simple repo that is used for understanding the basics of git and github.
Git is a version control system that is mainly used to track,maintain,control and save the changes that are made in the source code in the application development
Github is a website that is mainly used to store the git managed repositories using git.


GitHub provides features like code sharing , pull requests , collaboration.

(Day 1 - 26/06/2026)
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




