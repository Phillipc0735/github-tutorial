# GitHub Tutorial

_by Phillip Camu_

---
## Git vs. GitHub

##### **What is Git?**  
**Git** is a `coding` language which can be used in many servers for coding purposes.  
##### **What is Github?**
**Github** is basically a web based version of git, and is a place that can "host" and run git which offers all basic things that git does. 



---
## Initial Setup

**Alright lets "git" you set up!**  (Warning many git puns will be used)  
**1 -** Well first off, you should start off by creating a github account on **[Github.com](github.com)** (its free dont worry).  Once you're done creating your github account, lets start creating your SSH Key!    
**2 -** Go to [Github.com](https://github.com/), and click your profile icon in the top right. Then click the "Settings" button, which should look something like this: (Add screenshot)  
**3 -** After you click settings, navigate to the SSH and GPG section on the left sidebar. (Add screenshot)   
**4 -** After getting to the SSH and GPG section, click the "New SSH Key" button on the top right of the website right under your profile icon. (Add screenshot)  
**5 -** Next, you're gonna want to name it "cloud9" (DONT PRESS ADD SSH KEY YET)  
**6 -** After naming it, go to your cloud9 tab/page: [c9.io](c9.io) (considering you have an account already set up, if you don't make one!) and click the gear icon next to your profile picture and the plus sign. (Add screenshot)  
**7 -** Then, go to the SSH Keys section under billing & settings, and copy the **2nd** SSH Key and paste into your Github page, right under where you named the SSH Key. Should look something like this: (Add screenshot)  
**8 -** Now press add SSH Key!   
**9 -** Now go back to [cloud9](c9.io),(considering you have a github coding space set up, if you don't create one!) and open your workspace.     
**10 -** Click on the command line which should be on the bottom of the screen, and paste "ssh -T git@github.com", and the message "Hi (username)! You've successfully authenticated, but GitHub does not provide shell access._
"  
**After you've done that, you've finished your initial set up! Let's get to setting up your first repo!**




---
## Repository Setup

**Alright lets "git" your first repo set up!**  
**1 -** Open your c9 workspace, and find the `command` line.   
**2 -** Just to make sure, lets cd into your workspace/go to your workspace by using the command: `cd ~/workspace`  
**3 -** Next, lets make the directory you will turn into a repository by using the command: `mkdir first-repo`  
**4 -** Alright now that you've made the directory, lets go to it by using: `cd first-repo`  
**5 -** Lets initialize/put git into your directory to turn it into a repository by using: `git init`  
**6 -** Alright now lets add the first file to the repository.




---
## Workflow & Commands

**`Git Init:`** Initializes git (coding system) in our directory (now called a repository) -- only do once at the beginning (hire family photographer) <----- (Analogies to help give you a better understanding) **_NEVER DO GIT INIT IN WORKSPACE_** (Fix to this problem is below)   
**`Git Add . :`** Adds a file you have created to the stage (Adding someone to the picture but not taking the picture)  
**`Git Commit -m "message":`** Creates a snapshot of your code/files that were on the stage (Taking the picture with all people added) COMMIT MESSAGES ARE VERY IMPORTANT, Make your commit messages present tense and describe what was modified in the commit.  
**`Git Push:`** Pushes your commits to a remote repo. (A remote repo is basically a place where your data is sent to.)  
**GET USED TO ADD, COMMIT AND PUSH!**  
**`Git Status:`** Keeps you updated with your past commits, and your directory. **USE FREQUENTLY**






---
## Rolling Back Changes
**These commands will help undo pushes, commits, adds and edits just in case you make mistakes.**

**`Git reset --soft  HEAD~1:`** Undos the commit or "snapshot" but keeps the files that were added on the stage.   
**`Git reset HEAD~1:`** Deletes the commit and takes file off the stage.  
**`Git reset --hard HEAD~1:`** Deletes the commit, add and edits made to the file. 