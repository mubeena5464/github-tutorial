# GitHub Tutorial

_by Mubeen Alam_

---
## Git vs. GitHub
**_Git_** is a type of `verion control`. A `version control` is a system that records the changes being 
mad on a file in this case our repositories. Git screenshots the coding and it does not need 
internet to run. It runs in your `local` computer. Git does not need GitHub to run. Git is used by all 
developers. Git is in your command line. After you are complete with making your directory. you can just 
`git add` and `git commit` we will get more into that in Workflow & Commands.

**_GitHub_** is the cloud that contains the repositories. This helps save files incase something goes 
wrong on the local machine. GitHub has to be run by Git. In this case internet in required to connect
to the cloud. GitHub can be usefull if a person needs to share his or her files with another person. 
GitHub is the `remote`. 



---
## Initial Setup
For using GitHub you need to go to [Github](http://github.com)  
Make an account and sign into your account.  
Set up `SSH key` to connect GitHub with your command line.  

For an example on [Nitrous](http://nitrous.io)  
  1. Go on username  
  2. Dashboard  
  3. SSH Key tab  
  4. copy SSH Key  

On GitHub   
  1. Go into your profile.  
  2. Go into Settings  
  3. Go to SSH keys  
  4. Click on Add SSH Keys      
  6. Give it a title (example: Nitrous)  
  5. Paste your Key   
Once you are in your container open IDE  
 
And now you have to *_Start Coding_* on your command line   
`ssh -T git@github.com`  and type "yes"    
Now you have to `git config`:  
First make a dirictory:  
`mkdir first-repo`  
`cd first-repo`  
`pwd` to check where you're at  
you should be at /home/nitrous/first-repo  
`git init`  
`git config --global user.name “First Last”`  
`git config --global user.email “your email”`  
####You are command line is now coonected with GitHub.





---
## Repository Setup
`pwd` to check where you are  
You should be in /home/nitrous/first-repo  
There should be `(master)` writen next to it confirming that you are using Git  
`touch README.md`  
open the README > WHATEVER YOU WANT TO WRITE  
For Nitrous you have to manually save.  
`git add README.md`   
git commit -m “commit message (ex; add readme)”  
Back in GitHub go to the `+`  
New Repository  
Repository name: first-repo (has to be the same)  
Create Repository  
Click SSH next to URL  
Copy the `git remote`  
Now copy the `git push`  
Now refresh your GitHub page and you should be able to see the changes.  
From now you just work on you README.md 
Add and Commit  
And `git push` no need for the `-u orgin master`




---
## Workflow & Commands  
`git` a git command  
`remote` we are setting up a connection between our current repository and an external one  
`add` to add a repo into file   
`origin` this is our “nickname” for the remote repo.
`URL` the location of the remote repo.    
`push` we are sending our commits from our local repo to our remote repo  
`-u` means “upstream.” This remembers which remote repo & branch to push our changes to when    
we type “git push” in the future.  
`origin` this is which remote we are pushing to  
`master` the “main” branch of your project   
`pull` bring any changes from the remote to the local   
`git init` initializes git in our directory/repository for version control, only do this once
at the beginning  
`git status` optional command to see which files have been edited since the last commit    
`git add file.ext` add the file(s) to the stage to be committed   
`git commit -m “short/specific message”` take a ‘snapshot’ of the files on the stage.
The message should be present-tense and describe what was modified in this snapshot   
`git log` see your past commits  
`git diff` see the difference between your current code and the previous commit
