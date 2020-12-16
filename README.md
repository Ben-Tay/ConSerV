# ConSerV

GitHub Repository for ConSerV 
**(Refer to https://dzone.com/articles/top-20-git-commands-with-examples for some examples on git commands, otherwise look at the git docs)**

**Section A: (Only applicable to repository owner)**

[Upload existing project to GitHub repository:

1. git init  (initializes empty repository)
2. git add . (adds all files that have been changed to commit list)
3. git commit -m '' (commits all added files with a message)
4. git remote add origin git clone https://github.com/Ben-Tay/ConSerV.git
5. git push origin master 

**Section B: Apart From Section A, Rest all applicable to everyone
Remember all git codes should only be done in the project folder - ie : D:\IonicApps\ConserV
Section B should typically only be done once upon first importing of repository and creating of branch

[Import codes from Github repository into local environment:

1. git clone https://github.com/Ben-Tay/ConSerV.git
2. git pull origin master (may or may not need on first time you import to your local project)

[Create your own branch:

1. git checkout -b <branchname> (note that <> is not required when you write in your terminal)
2. git checkout master (switch back to master branch) - not rlly required usually (just showing you how to switch between branches)
3. git checkout branchname (switch to any other branch)

**Section C: (For every) - remember Section C onwards must be done in your own branch

[Everytime u make changes in your own branch and want to push your codes to github in your own branch:

1. git add . (adds all files that have been changed to commit list) or git add ../.. (path of file if you do not want to add all files that have changes)
2. git commit -m 'hello' (commits all added files with a message)  
3. git push origin yourbranchname (pushes your codes to your branch)

**Section D: Branch Merging

[Each time you want to make a pull request (merge your branch to the master):

1. Assume u have done the steps for Section C already with everything for the feature you are working on done.
2. git pull origin master (updates your branch/own local project with the integrated codes)
   (Will not affect your codes unless someone else has touched the file you have worked on and merged their changes into master - this may result in a merge conflict)
   (We often advise to do git pull origin master regularly even if not merging yet so that your branch wont be behind by the master by a lot of commits)
3. Assume you have not faced any merge conflict, do git push origin yourbranchname again after updating local project with master branch
4. make a pull request for your branch(it will be shown on the Github repository site itself)
5. select a reviewer who will go through your codes and decide if you should make changes or merge your branch to master


[Assume you face a merge conflict after git pull origin master: (Feel free to ask us if you meet issues with this)]

1. Resolve the merge conflict 
(Merge conflict errors will be shown in your own local project - you have to resolve them by deleting the lines in files that are stated to have errors in your terminal. 
(Search the internet to see how to resolve)
2. git add .
3. git commit -m ''
4. git push origin your branch name
5. make a pull request for your branch(it will be shown on the Github repository site itself)
6. select a reviewer who will go through your codes and decide if you should make changes or merge your branch to master

**Section E: Helpful Git Commands**

1. git status (checks added files or files to be committed)
2. git branch (checks what branch you are on)
