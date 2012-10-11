# Instructions for Using Git
** Note that you need to sign up for a free account at github if you have not already done so **

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
The key you created in the "Initial Setup" steps above gives your computer permission to send and receive data to and from your repositories on github. 

## Pushing your Changes Up to Github


## Terminal Tips

### Tab Completion
Any time you hit the tab button while typing in terminal, the system will try and auto-complete what you are typing. For example, let's say you create a folder called "myprojectwithareallylongname". Try it now:
1.  type `cd ~` to go to your home directory
2.  type `mkdir myprojectwithareallylongname`, which creates a folder called myprojectwithareallylongname
3.  type `cd  mypro`, then hit tab, and you'll see tab completion at work

### Usefull Commands
- `ls` gives you a list of all the folders and files in the current directory
- `ls -a` gives you a list of all the folders and files in the current directory, including the hidden files and folders
- `cd` allows you to change the directory and move around the file system
- `mkdir foldername` creates a folder with the foldername in the current directory
- `touch filename.txt` creates a file with the name and extension you specify
