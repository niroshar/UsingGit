This file contains steps using GitBash editor

- To change a folder 
$cd folderName

- To go back one step in folders
$cd ..

- To see the list of files in the current folder
$ls 

- To check the path 
$pwd

- To initialize a git project(repository) in the current folder
$git init

- To see what is in this repository and all the hidden file
$ls -la

- Create a text file in text doc and save it in the current folder 

- To add the changes to the project and enter 
$git add .

- You need to commit to GitHut
$git commit -m "This is the first commit"

- Do changes in the previous created file and save text file. after making changes commit it adding a msg with what you have changed.


- How to view your commit history
$git log

- To view other people's commits (you don't have to enter the whole name, entering only a part of the name is enough)
$git log --author="nirosha"


- To understand how changes are made
$git status 

If it says "On branch master, nothing to commit, working tree clean" meaning that there are no changes done


* If you have done any changes it will show what are the changes when you type $git status. This will work only if you have commited the folder before.

- To add another file to **staging area** , Note that this file is not yet saved in the repository. You have to commit this file to see the file in GitHub account.
$git add filename.txt


- will be 
$git status 

- to commit
$git commit -m "adding the second file"

$git status

- How to view the changes that made to a file
$git status 

Then it will show in red text while file is edited but it is not commited. 
When you enter the following command in GitBash it will show the content of what has been changed.
$git diff

- now commit the change as follows
 $git commit -m "commiting the changes"
 
 * check again $git diff then nothing will be appear after commiting the changes made.



