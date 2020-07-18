### [HOME](https://krishna-waidande-dev.github.io/)

# Getting Started With Git

## Installation

First install git on your machine .

I am using ubantu so I run this command in my terminal
``` apt-get install git```


To install git [Click-here](https://git-scm.com/download/linux).

After installation of git on local machine.

Create a account on [Github](https://github.com)

After creating account on Github, you will see a window on that window look on right upper corner of navigation bar.

> You will see + sign click on that sign choose new repository option.


> Now give a repository name same as your project name (optional but good habbit to keep same name as project name).


> After that just click on create repository button.

### How to use git.

Once done now Open terminal.


Go to a folder in which you will create your all projeect files.
suppose I want to create my project in DemoProject folder which is located on my desktop just get in that project


For example : 

```
user@user-Lenovo-ideapad-320-15ISK:~$ cd Desktop/
user@user-Lenovo-ideapad-320-15ISK:~/Desktop$ ls
CRM  DemoProject PYTHON  reports.sql  StoreDB.sql
user@user-Lenovo-ideapad-320-15ISK:~/Desktop$ cd DemoProject/
user@user-Lenovo-ideapad-320-15ISK:~/Desktop/DemoProject$ 
```

Now you are in a project folder where you want to clone a github repository.

> Clonning directory means sinking our local repository(folder) with remote repository(your git repository).

now on teminal just before typing a command just go on your github page and copy the url.

for exmmple :- https://github.com/krishna-waidande/DemoProject.git


and now on terminal type following command and hit enter.

```
git clone https://github.com/krishna-waidande/DemoProject.git

```
After typing this command just type ```ls``` you will see a folder is created in your local machine name will be same as your remote repository name. 

```
user@user-Lenovo-ideapad-320-15ISK:~/Desktop/DemoProject$ git clone https://github.com/krishna-waidande/DemoProject.git
Cloning into 'DemoProject'...
warning: You appear to have cloned an empty repository.
user@user-Lenovo-ideapad-320-15ISK:~/Desktop/DemoProject$ ls
DemoProject
user@user-Lenovo-ideapad-320-15ISK:~/Desktop/DemoProject$ cd DemoProject/
user@user-Lenovo-ideapad-320-15ISK:~/Desktop/DemoProject/DemoProject$ 

```

  In above example DemoProject is name of my remote repository (Github repository) . 

  Get into that folder by typing ```cd <repository name>``` as show above.
  
  Now You can create your project Folder files/folder in this folder.
  
  Now we will see 
  #### how to add a text file into remote repository.
  
  create a text file once created just type following commands .
  
  +  git add <filename / folder name> : To add files to remote repository.
  ```
  user@user-Lenovo-ideapad-320-15ISK:~/Desktop/DemoProject/DemoProject$ git add DemoFile.txt
  ```
  
  + git commit -m "initial commit" :- This is used to commit added files to server.
  
  
  ##### -m is used for givimg messege for our commit and it ia compulaory to give proper commit messages.
  
  
   ```
  user@user-Lenovo-ideapad-320-15ISK:~/Desktop/DemoProject/DemoProject$ git commit -m "My initial Commit"
  [master (root-commit) efc3358] My initial Commit
  1 file changed, 1 insertion(+)
  create mode 100644 DemoFile.txt
  ```
  
  + git push : to push our local file / folder to remote repository.
  
  > while pushing file it asks for your username and password just provide username and password of your github account.
  
  ```
  user@user-Lenovo-ideapad-320-15ISK:~/Desktop/DemoProject/DemoProject$ git push
  Username for 'https://github.com': krishna-waidande
  Password for 'https://krishna-waidande@github.com': 
  Counting objects: 3, done.
  Writing objects: 100% (3/3), 254 bytes | 254.00 KiB/s, done.
  Total 3 (delta 0), reused 0 (delta 0)
  To https://github.com/krishna-waidande/DemoProject.git
  * [new branch]      master -> master
  ```
  After push you can go to your Github  account and refresh the page you will see your file there. 
  
  
  #### Note :- for now we are adding files to master so you can use ```git push``` coommand as it is . but if you want to add your file to another branch you need to run this command.
  ``` git push origin newBranchName```
  
  
  
  + git branch :- telles us on which branch we are.
  ``` 
  user@user-Lenovo-ideapad-320-15ISK:~/Desktop/DemoProject/DemoProject$ git branch
  * master
  ```
  
  git pull :- to fetch files or folders from Remote repository. 
