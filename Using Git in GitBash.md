


To change a folder 
`$cd folderName`

To go back one step in folders
`$cd ..`

To see the list of files in the current folder
`$ls` 

To check the path 
`$pwd`


### (1) Create a folder in your local drive for existing repository

First, go to the folder in your local computer. Then you should use the command *git clone* and give the path of your repository in Github.com. 
Ex: git clone https://github.com/username/repo.git

This will make the connection between your local folder and the repository as well as will download the files if you already have uploaded some files to your github repository. Now, you can start moving your files from local computer to `GitHub` repository. 

### (2) Initialize Repository
Suppose that you already have created a folder in your local computer, then you should initiate the folder before adding files to the staging area(to be committed files). Open `Git Bash` command prompt and change the path the current folder using `cd PATH` command and initialize the path using `git init` command.


### Upload files to the repository
If (1) or (2) are completed, now it is time to add the files to the repository: use `git add filename` if you want to add one specific file or `git add .` to add all the files in that folder. Use `git commit -m 'write your comment here within quotation marks'`. You can use `git status` command to see the status of the added file which tells about the files in the staging area. Now you use `git push`command to push the file to the repository. It will ask to enter your `GitHub` account user name and password. 

Now, you can make any changes to the files in your local computer, use the same procedure to upload the files to the repository. If you have done any changes it will show what are the changes when you type `$git status`. This will work only if you have commited the folder before. After adding the file, use `git status` to check the staus, it will show the file name in red text while this file is edited but it is not commited (It is in **staging area**, not saved in the repository yet). You have to commit this file to see the file in GitHub account.

*Note that* every time you make some changes to the files in our local directory, it is needed to **commit**, and **push** in order to upload the edited files to github repository. Remember to add a comment when you commit, so that other people can easily figure out what changes you have made to that file.


### Upload a folder to the repository

Suppose that you already created a repository in `GitHub.com`. Now, create a new directory in your local computer and copy the folder to that directory. Use `GitBash` to change the current directory to this new directory.

Now it is time to initialize and add the folder to `GitHub repository`. Use the following commands in GitBash 

- `git init`
- `git add folderName`
- `git commit -m "Include your own comment"`
- `git remote add origin https://github.com/username/repoName.git`
- `git push -u origin master` 


Now go and refresh your `GitHub` profile, the folder will be uploaded into the corresponding repository.


**Some Commands**

When you enter the following command in GitBash it will show the content of what has been changed.
`$git diff`


To see what is in this repository and all the hidden file
`$ls -la`

 Create a text file in text doc and save it in the current folder 

To add all the changes to the project
`$git add .`

To add changes in one file
`$git add filename` 

How to view your commit history
`$git log`

To view other people's commits (you don't have to enter the whole name, entering only a part of the name is enough)
`$git log --author="nirosha"`


To understand how changes are made
`$git status `

If it says `"On branch master, nothing to commit, working tree clean"` meaning that there are no changes done

 * check again $git diff then nothing will be appear after commiting the changes made.
 
 
### Create GitHub Repository

Now, you may go to your github profile and create a new respository using `+` sign with down arrow next tp your profile lego as shown below:

 ![Create a repository](images/repoCreate.png)
 
 
 Next, you will see a weblink related to that repository, which starts with `https://github.com/username/repoName.git`. Now it is time for you to upload your files into your github account. First, you should add the file, then commit as I described above. Once it is done, you can link the file to repository in the GitHub. In order to do that, go to GitBash and give the link of your repository.
 
 `$git remote add <NickName> https://github.com/username/repoName.git`
 
 After that, you need to push it to load it into your GitHub account using following command in GitBash. You will be asked to enter user name and password for that.  When it is done, you can check the $git status to see any files are in the **Staging area**.
 
 `$git push -u <NickName> master`
 
 * If you haven't selected to create the **"README.md"** file when creating your repository, you can create the **"README.md"** as follows
 
 `$echo "# repoName" >> README.md`
 
 `$touch README.md`
 
 `$git add README.md`
 
 `$git commit -m "README.md edited"`
 
 `$git push <NickName>`
 
 `$git status`
 
 



