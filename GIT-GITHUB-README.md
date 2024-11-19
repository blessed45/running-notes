GIT AND GITHUB 1
================
                 
Software Development lifecycle (SDLC)
-------------------------------------
Develops, Tests, Builds, deploys & monitors applications 
Applications are the output from Software

Releases:
-
Releasing an application is taking/deploying it to the client.

In realtime we have multiple Releases.

release1 = version1   = 1000lines of code  
   echo 'Hello'

release2 = version2  = 2000lines of code  
   echo 'Welcome to Paypal'.
   
   echo "Your convenient payment gateway".

Release3  = version3  = 1000 lines of code  
echo "Paypal the best payment gateway"

Rollout   --> version1 --> version2 ---> version3  
RollBack  --> version3 --> version2

The client is not happy with the latest version of the application.   
What can be done??? We RollBack

Versioning in Software Development:
===================================
Version control systems = VCS:

  Local = version1,
  
  version2,[5000LINES ] 
          
  version3 [2000LINES ] 

cons:
-
1. Single point of failure
2. lacks collaboration
3. in-efficient use of resources including time  
4. can't RollBack  
  

Apart of the local system, we also have what is known 
as the centralize system;
With this kind of a system, there is a central system,
i.e
   we create a server, where when developers write their
   codes, they can commit it to the server and save it there
Here, there is a level of some collaboration, but the major
problem here is that, we can't rollback and the server can
go down (fail at anytime), so this method is also not really
secured

  Centralised:
  cons:
  -
-can't RollBack

-The central server can fail. 

To that effect, we have what is known as the distributed version
control system.

GIT => distributed version control system (DVCs)

Git manages data as snapshot
----------------------------

It takes a picture of what all your file looks like
at that and stores a reference of that snapshot 
And we can make a reference of that snapshot.

With Git;
Developers can collaborate

Here, we have a distributed version control system

     For each developer, we have to make sure that Git is install
     in their local environment.
     And they can write codes and commit it to the remote server 
     and that remote environment is known as GITHUB

Github is a source code manager (SCM)

Github => SCM

With Git;

- nearly every operation is local
- Git has data integrity
- Git generally only add data
- we can rollout and rollback with Git

* data integrity => when developers commit codes in Git/Github,
  we can know who actually committed the code and if there are any 
  changes and who did the changes in the  code or software


Other version control systems includes;
--------------------------------------

      - SVN => Subversion
      - CVS => Concurrent version system
      - TFS => Team foundation system
      - GIT => 95% of companies are using GIT

That is why we will be using Git

Git is a distributed version control system

In our environment, we use Git for versioning

And if we are going to be using Git for versioning,
Git comes with a source code manager known as Github

    Github = source code manager

In the developers environment, a command line known as
GitBash is installed, this is because when you install Git,
it comes with a command line known as Gitbash

So before codes are commited from the local environment to
the source code manger (SCM), Git is already installed and applied

When it comes to source code managers (SCMs), 
We have different source code managers platforms and these include;

   - Github
   - Gitlab
   - Bitbucket (stash)
   - Awscode commit

IQ
--
   As a devOps engineer, what are your roles and responsibilities in
   versioning with Git?

ANSWER
------
    
    1) 
      - We ensure that developers environments are configured and secured
      - We create an enabling environment for developers to code/develop
      - We ensure that development servers are created in AWS/GPC and secured
      - Login details shared with developers/team
               usename
               password
      - We ensure that Git package/software is installed
                
    2) Project onboarding
             
      - Create organisations where applicable in a SCM (Github)
      - Create repositories in the SCM (Github)
      - Create teams in SCM and assign members (developers , etc)
      - Create Github account for your organisation

Git Download
------------
For you to connect to Git, the website is;

      website = httpw://github.com/

creating an account in Git requires;
-
- name
- email
- username
- password
- 
After creating an account, you can now login
using;

- username
- password

How To Create An organisation
----------------------------

   - Go to the top right while in your Github account
   - Click on the + sign
   - Select new organisation
   - Entered the required information to create an organisation
   - Copy the organisation URL

How To Create A Team
--------------------

    - Go to the organisation that you created and click on it
    - On thje top bar, click on teams and select new team below 
      in green coloration
    - Enter team name, description.
      select visible
      e.g
        teamname = paypalteam
        description = paypal
    - Copy the team URL

How To Add Members To A Team
----------------------------

For members to be added to a team, either one of the following is needed

            - account username
            - email
This is only possible if you have a Github account
If either of the above information is provided,

Go to your team dashboard and select, [add a member] in green coloration,
enter the github acount username or email of the mamber you want to add in the 
search bar and click on invite
After doing that, ask the member to accept the invitation
once that is done, the member will automatically be added to the team

How To Create Repositories For A Team
-------------------------------------

     - Go to the organization dashboard, on the top bar, click/select repositories
     -Create a repository for the organization.
     -Go back to the organization dashborad and select team 
     - Click on [add repository] in green coloration
     -Enter the repo name that you want to add to the team, on the saerch bar.
     -Select add repository 
     

     when you do that, you will see an add repository, to what so ever team 
     that you created search bar box, add a repository to that repository,
When members of the team write codes, they can now collaborate

OR  

You can go to the organization that you created,
on it's dashboard you will see [create a new repository], click on it
enter the required information

            repository name - paypal
            Description - paypalrepo       

select if you want the repo to be public or private

NOTE;
-----

      public repo can be viewed by anybody in the world
      private repo can only be viewed by you or members of your team

    - Copy the team-repo URL
    
 At this point, we have some URLs that we have created
 i.e
     - organization URL
     - team URL
     - organization project-repo URL

So as DevOps engineer, you can be task to create:

   - a github account for your organization
   - create team and add members
   - create project repo in the organization for members
   - grant permissions and roles to members and collaborators
   the kind of permissions granted include,
read  - can only read or view codes
write - can read/view and make changes
admin - can do all
For this to be achieve,
           go to organization, under it , go to team and under settings
           select [member privileges]
         the member privilege page will display and under it there is a
         base permission page where member's permissions can be set

         when this is done, the project repo can now be shared to members os
         the team where they can now write codes and push them to

   - ensure that git and relevant IDEs (integrated development environments)
     are installed by developers

Git Installation
================

Git installation differ depending on your operating system

      windows --> install gitbash
                 https://git-scm.com/download

                 once you install git, it will come with a 
                 gitbash terminal

      RHEL servers --> 

          sudo yum install git -y

          git --version -> check version of git installed

      ubuntu linux servers -->
      
          sudo apt install git -y

          git --version -> check version of git installed

Now that we have successfully installed git, for us to start 
working on a project, we are going to be assummimg the rule of a developer.
In our local environment, we have to create a project directory

            mkdir projectname

navigate into the project directory

            cd project-directory            

when you do this, it is not yet a git repository, for you to create a local
git repository, run the command,

            git init

This commsnd will initialise the working directory that you created to a local
git repository

To check if there are any commits, run the command;
      
            git status

At this ponit, when you run this command, it will tell you no commits yet, this is
because there is no development taking place yet but the repository has been initialised

For you not to get the [no commits yet] message, 
  create a file in the project local repository

           touch projectfile-name

and add content to the file

re-run the command,

           git status

you will now see a file that is being tracked by git in a red coloration
at this point, the file is where we called;

          the working area

From here, the file can be move from the working area to the staging area by running the command;

          git add filename

when you do this, you have just moved the file to the staging area, if you run;

           git status

You will now see that the file is in red green coloration, written as [new file list]
At this point, we say the file is in the staging area
but take note that we have not yet committed the file/changes to the staging area

For us to commit the changes/file to the staging area, we run the command;

               git commit -m

               -m = good commit message

      e.g
           git commit -m "my first commit"

When this is done for the very first time, a message [please tell me who you are] with an authentication file,

         git config --global user.email "email"
         git config --global user.name "yourname"

Copy the first authentication line and edit it with your email address
i.e 
      git config --global user.email "your emailAddress"

then run the whole of that command

Copy the second and edit with your github account username,

        git config --global user.name "your github acct username"

 Run the command also,
 

 By doing this, you have created what is known as global configuration and you have to do
 that with your own information
 This is so bscause you cannot commit if you are not yet known by the system

 This is for data intergrity
 Remember we discussed about data intergrity
So we can track who is doing what using thier email address and name

At this point, we can check the number of commits that we have by running 
the command;
     
            git log

After running the command to check the number of commits, a message will be 
display as follow
    [Your current branch 'master' does not have any commit yet]

Since you have configured your global configurations and is now known by the
system, you can now commit changes/files with relative else, re-run the commit command;

            git commit -m "commit meaage"

If you  now run the command;

           git log

The commit ID will be diplayed to you
git comit have moved the file/changes, with a good commit message to the staging area
[local repo]

There are few commands to take note of;

- git commit -m -> creates a version with a version number [commit + ID]

- git init -> initialises a git empty repository abd create the default branch [master, main]

- git status -> tracks file location

- git log -> list all commits with commit ID

- git add -> move files from working area to staging area

- git commit -m -> move files from staging area [local repo] with a good commit message for
                    tracking changes
                    creates new versions of applications


To know what happens to a particular commit, run the command;

            git show commitID

To check if there is any repositiry detail in the local environment, 
run the commd;
              
              git remote -v

To add a repository in the local environment,
run the command;

              git remote add aliasname repo-url

when ever this is done, the alias name will now represent the repository url

e.g 

          git remote add paypal rep-url

paypal will now represent the whole of that url                        



GIT AND GITHUB 2
================

All these while, we have been discussing that our task as a DevOps engineer
include;

     Developing applications
     Testing applications
     Building applications
     Review and qualifying applications
     Deploying applications
     secure applications
     Monitoring applications 

i.e. 
    Being able to manage applications irrespective of it's complexity              

In our last class, we started seeing how we develop and push files to a remote
repository in the source code manager(SCM) GitHub,

Before we did that, we ran some few commands and we are to take a review of the
commands that we have been executing so far with git and GitHub ;

- git commit -m -> creates a version with a version number [commit + ID]

- git init -> initializes a git empty repository and create the default branch [master, main]

- git status -> tracks file location

- git log -> list all commits with commit ID

- git add -> move files from working area to staging area

- git commit -m -> move files from staging area [local repo] with a good commit message for
                    tracking changes
                    creates new versions of applications


To know what happens to a particular commit, run the command;

            git show commitID

To check if there is any repository detail in the local environment, 
run the command;
              
              git remote -v

To add a repository in the local environment,
run the command;

              git remote add alias name repo-URL

when ever this is done, the alias name will now represent the repository URL

e.g. 

          git remote add PayPal rep-URL

PayPal will now represent the whole of that URL                        

- git push = pushes the commit from the staging area [local repo] to the remote repo
             in GitHub

so today, we will continue to see how workflow is being achieve with git
Following what we discuss in our last class, we said;
    git is a distributed version control system use in tracking files
    i.e.
       git is use for versioning

Let us now look at how files can be modified in Gits

For us to modify a file,
e.g.
    if we run the command bellow to append a new content in an old file,
    i.e. 
      modifying the file

      echo "message" >> file
OR
      vi into the file and add content

where; 
   message = new content you want to modify
   file    = the file you want to modify

When you do this, run the command 

           git status

You will see a modified file in red coloration
Run the command,
     
           git add .

 where,

      . = you present working directory
i.e.
   you want add all the changes in your present working directory
   to the staging area

When you do that, run the command;

         git commit -m "commit message"

To commit the changes to the staging area 

Check if the changes were successfully committed to the staging area
by running the command;

           git log

But note that, at this level, the changes have not yet been committed
to remote repository

So if you run;

           git status

The system will tell you;

              nothing to commit, working tree clean

For these changes to be committed from the staging area [local repo]
to the remote repository, we run the command;

             git push

i.e.

      git push <aliasname> <branchname>

 e.g.
 
      git push fintech master

That is, if the changes are being pushed to the master branch,
but if you want to push to the development(dev) branch, stage
branch, feature branch, or any branch that is found in the remote
repository, you have to make sure that you specify the branchname.

When you do that at the very first time,
It will request for your username and password

Here, password has been deprecated
i.e.
   password is no longer accepted by the system

So in the place of the password, we will be using an authentication token.
This is because Git no longer support password authentication

To achieve all these;

- Go back to your GitHub account
- Go to settings
- Scroll down to developers settings
- Choose personal access token
- Select token(classic)
- Click on generate new token token
- Select generate new token (classic)
- Enter the required information to create a token
- Click on generate token
-Copy the created token

Now go back to you CLI
Where there is the password authentication, enter the token you created
And make sure you user name is that of your GitHub account

i.e.

     username for 'https://github.com':<enter your GitHub account username>
     password for 'https://yourname@github.com':<enter the token you created>

Once you are authenticated, you can now push your changes to the remote repo
with relative ease.

ASSIGNMENT
---------
Project,
--------
1) Create your GitHub account and onboard a new project for a fintech client

2) Create a team in your created organization for PayPal and add members 
   of your group with write access 

For you to obtain a new project,
As part of the onboarding
 you may require to;

- create an organization
- create a new team
- add members to the team
- create a repository

We realize that when applications are developed, they have different
versions, So we need a distributed version control system to manage
this process. And we saw that Git as a DVC has a lot of advantages,
Which include;
   
  - Enabling collaborations
  - Permits rollout and rollback
  - Save time

  We saw how git can be install in windows

Let us now look at how Git can be install in Linux

For us to install git in Linux, we need a Linux server
We saw how to create Linux base servers in our Linux classes 
and how to connect to the servers with relative ease,

So for you to install Git in Linux

Connect to the Linux instance(server)
Run the command;

      sudo yum install git -y
      sudo apt install git -y

Check the version of git installed by running the command;

      git --version

Now that we have installed git in Linux,
Let us look at how we can carry out some few task;

We start by creating a project directory using the command;

          mkdir <project-directoryname>
          mkdir <directoryname>

After creating the project directory,
Create a project file the directory, using the command;

          touch <filename>

Add content to the file, either by;

     echo "message" >> file

OR
    you vi into the file and add content

        vi file

Don't forget what we are doing is assuming the duty of a developer

let us create another file by using the command;

        touch filename

Add content to the file

There are some git add commands that we must take note of;

          git add filename
          
          git add . 
          
          git add *        
When ever we have some file in our working area, to move one of the files
to the staging area, we use ;

           git add filename

But if we want to move all the files from the working area to the staging area;
We either use;

          git add .
or
          git add *

After we do that, we now configure our Global Configuration
This is because if we try to commit without Global Configuration,
The system will ask us to do that.

At this point, if we check to see if there is a commit in the remote
repository, we will see that we don't have any remote repository, so
we have to run ;

           git remote add aliasname repoURL

e.g.
           git remote add fintech project-repo-URL

After adding this project to the remote area you can check by running;

                 git remote -v 

And you will see an attach URL to your project repository 
i.e.

       fintech https://github.com/fintech-1/fintech-repo (fetch)
       fintech https://github.com/fintech-1/fintech-repo (push)

At this point , you can now push the changes to the branch you want to
in GitHub.
i.e. 
         git push fintech master

Take note that we have master because we want to push to the master branch
as specified by the example

TAKE NOTE;
---------

     working area        --> untrack files
                         --> in red

     staging area        --> git add
                         --> in green

     local repo          --> git commit
     
     remote repo(github) --> git push  

In real time, when developers are writing codes using GitHub
as a source code manager (SCM), they collaborate with each other,
what they do is that, when one commit change to GitHub using the 
git push command, for others to work on the same code, they have
to copy the commit in their own working area, for this to take place;
they either pull or clone the code using the commands;

             git pull 

i.e. 
             git pull alias master
             git pull fintech master
OR
             git clone project-repo-URL
e.g.
             git clone https://github.com/fintech-1/fintech-repo

When this is done, they will now have a copy of the project code 
in their own working area.
when ever you clone a repository and want to see who did the last
changes on the code, cd into the project and run the ;
     
                git log

For another collaborator to push commits to the remote repository,
He/She need to configure his/her Global Configuration by editing and
running the bellow command;

           git config --global user.email "email"
           git config --global user.name "yourname"

When this is done, he/she can now push changes made in the code to the
remote repository in the source code manager (SCM) GitHub, by running;

            git push alias branchname

In git, we have what is known as a branch

Branch = a branch is a line of development

To check a branch in git, we run the command;
 
        git branch


GIT AND GITHUB 3
================

As DeVos engineers, our task is to;

     Develop applications
     Test applications
     Build applications
     Review and qualify applications
     Deploy applications
     secure applications
     Monitor applications                 

In our last class, we saw how we can assume the function
of a developer, in writing and committing codes to the SCM,
We equally saw how to modify codes,
Today, we will continue to look at how developers collaborate
when they collectively work on a project.

let us start by adding content to one of our files that we have been 
working on,
             
             echo "message" >> filename

after modifying the file, we can check the content by running the command;

             cat filename

Now we can equally check if we have any file to be tracked by git, by running the command,

             git status

When you run the above command, you will see a modified file in red
At this point, we can now move the file from the working area to the staging area by 
running the command,

               git add .

We can now commit the changes

      git commit -m "good commit message"

If we execute 

       git log

We will be able to see who did the first commit and who have done the second

If you execute git log in the environment of the person that clone the code and added content, you will see that the person has two commits in the log file while the first person has only one commit and in our GitHub account we have just one commit

For the first person to get the changes, the second person will have to push the code to GitHub, and the first person will then pull the code from GitHub to have the changes that was modified.

NOTE;

     The first person will not clone the code because he/she has the code already and needs only the changes that the second person did.

So the second person is going to push the code, when he/she try to push the code to GitHub, the system will request for username and password and here the password is a personal access token, as we saw in our last class.
So, he/she will need to go and create a personal access token in GitHub and enter the token where the password is requested.

After pushing the code to the remote repository, we will see that we have two lines of code and the change will now be part of the GitHub project.

But in the first person's environment, he/she has just one commit, for he/she to ensure that his/her environment is in line, he/she has to pull the code,

            git pull aliasname branchname

After running this command, he/she will see a changed file with
  +1...N attached to it,
If he/she cat the file, the changes will be there

NOTE
     Git is all about versioning                     

To see a particular change that took place in a commit,
we run the command;

          git show commitID

Some Git commands that we have looked at so far include;

          git init
          git add
          git add .
          git add *
          git commit -m
          git remote -v
          git remote add
          git status
          git log
          git push
          git pull
          git clone
          git config
          git --version

These are very important commands to take note of.

GIT BRANCH
==========

In  Git, a branch is a line of development

e.g. 
           Development branch
           Stage branch
           Master branch

When developers are working, they usually use the development branch, 
when they are satisfied with their work, they can now push it to the 
stage branch, stage branch is created from the development branch and 
from the stage branch the code id then pushed to the master branch.
The same files are in all the branches
so codes from the development branch is being deploy to the Development
environment and that of the stage branch are being deployed to the testing
or QA or UAT environment and codes from the master branch are being deployed 
to production  
i.e.
          Dev branch    --> Development environment
          Stage branch  --> Testing/UAT/QA environment
          Master branch --> production

Let's look at what branches is all about.
Normally in development, it is good to have multiple development
lines so that if there is problem, with one line, we can go to the
other line(branch) to resolve the problem

CREATING A NEW BRANCH
=====================

Ticket 001 
----------

- Create a Dev branch from the master branch
- Switch to the Dev branch and create an app.java file
- commit the changes and switch to the master branch
- Review the changes in the Dev branch and merge with the master branch 

ANSWER
------

- To create a branch in Git, we run the command

            git branch branchname

e.g. 

            git branch dev

- To switch to dev branch, we run the command;

            git switch dev
            git checkout dev

To check the number of branches, we run the command;

            git branch

You can also use the git branch command to know the branch that 
you are working in

- When you switch to dev branch by running the command;

         git switch dev or git checkout dev

you can now create the app.java file and add content

If you run , 

         git log

You will see that you have some commits and if you run 

        git status

You will see a new file called app.java in a red coloration
If you cat the file, you will the content that you added.

This file is found in the working area in the dev branch,
If you run;
       
            git add .

The file will be move to the staging area and you can see that Git 
is tracking the changes.

If you run;

         git commit -m "commit message"

And run,

         git log

You will see that the new file app.java has been added to the log file

If you switch to the master branch

       git checkout master

and  run,

         ls

You will see that the number of files in the dev branch are more
than that in the master branch, this is because , there is a change
that took place in the dev branch that has not yet been merge to the
master branch, so if you execute git log in the master branch, you 
will see lesser files

To review the changes that took place in the dev branch, which are 
not in the master branch, run the command;

           git diff commitID

You will see the changes.
If the changes are in line with what you wanted, then you can now merge the changes in the dev branch to the master branch by running the command;

             git merge  dev

If you run git log in the master branch, you will now see that
all the changes in the dev branch has been merge to the master 
branch and if you run 'ls' , you will see all the files

NOTE

     The master branch is the upstream branch for the dev branch
     and the dec branch is the downstream of the master branch,
     This is because the dev branch was created from the master branch

To push changes to all the branches, run the command;

            git push aliasname --all

IQ
How many branches are you supporting in your project?
-----------------------------------------------------

ANSWER
------

    Branches are use to create lines of development in Git
    A branch is a line of development

    We maintain a minimum of three branches
          Development branch
          stage branch
          master branch

Some of the command that we again looked at include;

      git branch            --> list all the branches
      git branch branchname --> creates a new branch
      git checkout/switch   --> switches from one branch to another
      git fetch             --> it brings changes in the code to the local repo
      git pull              --> it brings changes in the code to the local repo 
                                and working area
      git clone             --> it brings the entire code to the working area

These are very important commands to take note of

NOTE
   We can create different branches from the master branch.
 e.g.     

      bugfix branch --> for bug fixes
      feature branch --> for future development

Codes from the master branch are deployed to production so the 
master branch is the most critical branch, so if you are carrying 
out a development, it should start in the list critical branch, 
which is the development branch.
So before you push to the master or merge code to the master branch,
the work must be well reviewed

PULL REQUEST (PR)
-----------------

Pull request (PR) is to review changes in one branch before merging in
another branch.
This recommended for any merge in the master/release branch

So if you want to apply changes in the master branch, do not do that directly
in the master branch, do that in different branches and review well before
merging to the master branch
