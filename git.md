[Back](/a-fro/newroots)
# Instructions for Using Git
**Note that you need to sign up for a free account at github if you have not already done so**

## Initial Setup Each Week
1.  Open up terminal on your computer (in Applications/Utilities)
2.  type `cd ~`, which will take you to your home directory
3.  type `ls -a`, which shows you all the folders and files, including hidden files and folders
4.  see if there is a folder called ".ssh". If not, then type `mkdir .ssh`
5.  type `cd .ssh`
6.  type `ssh-keygen`, which starts the key generation process
7.  type `enter` when asked to Enter the file to save the key
8.  type `enter` twice when asking for password
9.  type `cat id_rsa.pub` (use tab complete while typing if you'd like)
10. highlight what is in the terminal, starting with "ssh-rsa" but not including the new command prompt on the last line
11. Go to your account settings page on github (icon in top right)
12. Click on the "SSH keys" link in the left column, then the "Add SSH Key" button on right.
13. Give it a title (perhaps today's date), and paste the lines you copied in step 10 above.
14. Click the `Add Key` button.

## Creating your First Repo
Once you have an account on github, click on the "Create A New Repo" button in the top right. Create a public repo, with whatever name you choose, and also click the "Initialize this repository with a readme" checkbox before clicking the "Create Repository" button.

## Pulling Down Your Repository to your Computer
The key you created in the "Initial Setup" steps above gives your computer permission to send and receive data to and from your repositories on github. Use the following steps to pull down your repository
1.  type `cd ~/Documents` to get to your documents folder
2.  type `git clone git@github.com:[your git-username]/[repositoryname].git`, which will create a local folder with your repository name
3.  type `cd [repositoryname]`
4.  open sublime [installation instructions here](/a-fro/newroots/blob/master/sublime.md) or the program that you use for your programming environment (ie. Scratch) and begin working

## Pushing your Changes Up to Github
Before the end of each day, and better, throughout your work, you should commit your changes and push them to github.

1.  Type `git status` from within your project folder to see the current status of your repository
2.  If there are "untracked files" (files that you have created but not yet added to the repository), add them using `git add [filename]`
3.  Typing `git status` again will tell you there are changes staged to be committed
4.  Commit your changes to the repository, typing `git commit -m "A message about the details of the commit here"`. The -m stands for message, which is followed by the message in the quotations.
5.  At this point `git status` will tell you your local branch is ahead of master by 1 commit (or more, if you've committed multiple times without pushing)
6.  type `git push origin master`. "Origin" is the name of the remote location, in this case, github. You can see a list of remotes by typing `git remote -v`. "Master" refers to the name of the current branch you are working on. Therefore, "git push origin master" is an instruction to push the committed changes from your local master branch up to the master branch on github. 