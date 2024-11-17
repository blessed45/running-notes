                           LINUX 1 
                           =======

WHAT IS A CUMPUTER
------------------

A computer comprises of a hardware and a software component

the hardware components include
monitor, cpu, screeen keybord, mouise, harddrive, RAM, cards, motherbord

software component
1) os = operating system  == this is the principal software in a computer
2) other solfwares - office, adobe, antivirus

computers are manufacture by manufactureres and they include;
levono/ dell/ apple/ toshiba/ yoya/ samsung/ sony/ LG/ Acer/ HP   etc

CLASSES OF COMPUTER
-------------------
Computers are classified under;

personal class computers = these are computers used for personal use
-
these types of computers include; lenovo/ destop/ laptop/ phones/ notepads/ tablets/ watches/ ipads/  etc

enterprise computers;
-
they include; workstations/ servers (super computers)


what qualifies a computer is the OS
-
the operating system running in a computer defines the type;
examples of os include
linux/ 
windows/ 
solaris/
mac os/
ios/
android/

lenovo laptop is running with a linux os = linux system
HP ruunning with solaris = solaris system
dell with windows = windows system

is it possible for a computer to have more than onme opereting system?  the answer is yes
and you can also change the operating system form one to another and vice versa

WHAT DETERMINE THE CHOICE OF OS
------------------------------

1. SECURITY
       85% OF SERVERS ARE LINUX BASED
       linux systems are not vulnerable to virus attacks
       windows systems are vulnerable to varis attacks
3. COST
      linux is a free and open source OS
      windows is a licenced/paid OS
4. SUPPORT
         linux has a very large effective and free community support
         windows support is avalaible but paid only from mmicrosoft
         (vendor) 
5. USAGE
        LINUX OS IS MOSTLY UTILISED FOR ENTERPRISE TASKS
        WINDOWS IS UTILISED AS WORKSTATIONS 
6. PERFORMERS
7. REVIEWS
8. SPEED
9. SCALABILITY AND ELASTICITY


NOW WE WANT TO TALK ABOUT LINUX OPERATING SYSTEMS AND ITS IMPORTANCE
====================================================================
NOW;
   How are tasks runned or exicuted on a computer
   How are tasks perfomed om computer systems

Question
   For one or more of the following operating systems to run workload on computer systems;

We either use the GUI or CLI

1. GUI = graphical user interface
2. CLI = command line interface

what kind of workload can be exicuted on computer systems
we use computers to;

1 create files and content
2. modify files
3. create folders and directories
$. create sub-filders
5. sent emails
6. download filess
7. watch movies
8. create users
9. backup files
10. visit some websites
11. gaming
12. training
13. make money

HOW CAN WE USE A COMPUTER TO MAKE MONEY
---------------------------------------
1 GUI
    A fox using gui make like $65.000 per year
    they do jobs like
   administrative assistance/ customer service/ 

DEMO GUI

2. CLI
      to access the computer using commands, you need a command line
      The windows os comes with a command line called powershell
      MacOS comes with terminal as command line
      here you make like $230k upward a year

The person that uses gui take like about 20munites to create 20files while that of cli 
can take 3munits, so cli is more paid than gui users


LINUX OS AND LINUX COMMANDS
==============================

Linux is an open source operating system
Linux started in 1991 by LINUS TORLVADS

Linus was using the solaris system to carry out his project while at the university of 
Helsinki sweden,
Linus encountered a problem ruuning his project and and contacted the vendor but the res[ponds was delayed
solaris are licenced system, when Linus contacted the vendor and did recieve any respond, 
so he went ahaerd and created the linux sysrem by developing the solaris kernel
i.e He created the linux OS from the solaris kernel

Linux is an open sourse OS with multiple destributions/version
while windows/ solaris/ macOs/ etc are licenced OS

A solfware can be free / open source/ licence

1. Open Source
             Free with tghe source code
             Open source software has more community support
2. Free 
       its free but without the source coed

3. Licenced
           Paid for the OS

IQ
--
   Explain your experience with open source technology; linux
ANSWER
      With open source technology , the solfware is free including the source code (recipe/secret of the software)
DEMO
---
  You are invited by a friend for dina, you arrive and you served food and how the food was prepared, we can say here 
that you were served an open source food
another friend invits you for dina, serve you foor without telling you hiw the food was orepared, we say here that you 
were served a free dina
  this is the difference between an open source and free softwares


Since Linus developed linux and allow it as an open source OS, different companies were now able to use it and cto come 
up with their own OS
some of these include;
 1. REDHAT- red hat enterprice linux
 2. CentOs
 3. Ubuntu
 4. SuSe linux
 5. Fedora
 6. Gentoo
 7. Mandriva
 8. Slackware
 9. Amazon Linux 2AMI
10. Debian

TEH LINUX FILE SRUCTURE
=======================

Before we enter into the linux file structure, let us start by seeing how we can 
create and connect to a linux Os

CREATING A LINIX SYSTENM
------------------------
1. if you were going to create a linix system, you can either buy a server from the 
   market and configure the server
   cost = $50,000
   Time = 100x

2. You can use a hypervisor to create a linux vertual machine (VM) on your system
     cost = $3,000
     time - 10x

3. you can use a cloud computing provider 
              the cloud privider that can be use include;
              AWS/ AZURE/ GCP/ etc
  cloud providers provide for us computer services
        
laptop = 8GB?500ssd 
        cost = $500 - $1,000
        time - x      x=5 minutes

which of these will you prefer?

For us to create a linux OS we need an account in AWS cloud

CREATING AN ACCOUNT IN AWS CLOUD
================================

Requirements;
           website  =   aws.amazon.com
           email address
           password
           tel number
           credit card
 DEMO on hw to create an account in aws cloud

note that you will asked at the level of password to enter some special
characters, upper and lower case letters
e.g 
    ,,/ ../ ?/ #/ @ something like this for special characters


CREATING/LAUNCHING A SERVER/INSTANCE
====================================

After creating your aws account, you can nowlaunce a server, in linux we it an instance,
log into your aws console and search for EC2 , click on it and you will see an instruction
in a yellow coloration [LAUNCH AN INSTANCE], click on it , select the linux the OS you wish to use,
here we will be using RHEL [redhat enterprise linux] . go for the free version [free tier elligible] , 
click on it, scroll down, enter the name of the server you are creating, scroll down, in the password section, 
choose to create a key pair and enter the key pair. scroll down and launch the server/instance/, scroll up and 
click on instances, you will see the server/instance you launched in a pendind state, just wait fro some few 
seconds and you will see see a green running state coloration. that shows your server is up and running.
the key pair that you created will be downloaded into your computer, if you go to your download, you'll find
it there, and this is the key pair you will be using with the server ip to access your server
              
HOW TO CONNECT TO THE SERVER
===========================

To access the server you created, you need ;
            ipaddress of server
            username
            password/key pair 

CONNECT TO YOUR LINUX SERVER IN AWS USING SSH CLIENT/PROTOCOL
-------------------------------------------------------------

After creating an instance and obtaining the above requirements, for us to them to 
connect to our server that we created in aws, we need an ssh client solfware, 
Examples of ssh client/protocol solftware include; SSH = secured shall 
     mobaxterm
     gitbash
      etc
so for us to connect to our server we need to download the ssh client/protocol from its website
here we will be downloading mobaxterm
go to the mobaxterm website, click on the downloader and it will install on your computer, when it is 
installedm go to the start button and type mobaxterm, it will search for it, clicl on install and it will install 
a command line in you computer

Now to connect to our server, open the mobaxterm terminal click on the new session and take ssh on the top roll,
enter the ip address of the server, don't forget that whn ever an instance is launched, it comes witha user called 
[ec2-user] , so in the user colunm, enter ec2-user, click on advance settings , choose private key, don't forget that 
the kry pair you created was downloaded in the download of your computer, choose private key, click in it and double click 
on the key pair that was downloaded in your download, select yes and you will be connected to your linux server.
now you can start running tasks in the server

on your mobaxterm you can also choose local session ans run the ssh command as follows;
    
ssh -i keypair.pem username@server ipsddress
 
FOR MAC USERS/APPLE USRS DO THIS,

     chmod 400 keypair.pem = to ensure that your key is not publicly view
     ssh -l keypair.pem user@serveripaddress

those with mac computers should take note

After connecting the next thing to do is to start running tasks

Download the following solfwares
=================================
sublime text  =  this is a text editor
brakets       = text editor
mobaxterm     = ssh client software

you can download sublime text same way we did with mobaxterm


 THE LINUX FILE STRUCTURE
==========================

                      WINDOWS         LINUX
                    . fILES          .fILES         
                    . FOLDERS        .DIRECTORIES
                    .SUD-FOLDERS     .SUB-DIRECTORIES
ROOTS Directory       c:\                /
in the windows file structure, the principal directory is (c:) this implies that everything you do in windows 
begins with (c), while in linux it is a forward slash (/)
A directroy/folder is a container that contains files and sub-folders

LINUX FILE STRUCTURE
--------------------

linux root directroy = /

some few basic commands 
              
              ls  = list the content of a directory
              pwd = present working directory
              hostname = tell you the hostname of your server
if i run the command 
                  sudo hostname set-hostname demo  = it will change the host name of the server
to view changes, we switch to a user
                  sudo su - ec2-user 
now you will the our hostname has been changed

So now if we execute 'ls' which stands for list the content of the directory, 
       
           e.g     ls /
   
we will find out that the linux root directory has some content in it, lets run and see

DEMO 
    ls /   copy the content of it and explain the content of what is in the important directories

 e.g  

1) bin - contains binary files(commands) like ls, pwd, clear, cd, touch, mkdir etc
   
         Some other simple command that we will running include

             cd    =  change directory
             touch = creates a file
             mkdir = creates a directory
DEMO
    cd / and list its content with ls

home directory - contains users home directory details
     run the command ls /home  = this will list the content of the home derictroy

[ec2-user@demo ~]$ ls /home
ec2-user

now if we run the command - adduser = this will add a new user to our server
here we have learn another new command, lets try and see, not everybody can add 
a user to the server, so we need some privileges, in linux , we say you need root access
or sudo access, 
sudo simply means you are running the task as the root user
now if we run 
            sudo adduser emma
it will create a new user in our server called emma 
we can even add as many users as we wish, say; president, dominion, obi etc

if we now run the command ls /home, we will find that all the users we added to our server are 
stored in the /home directory
so lets now run ls /home and see what we have there

let us check at one other directory

2) sbin = this directory contain system binary files/commands
we talked about the bin directory containing binary files, similally the sbin contains binary 
file but these files/commands can only be executed by the admin users or root users 
e.g adduser, create passwd to users, change name of server etc


IQ
  what is the difference between bin and sbin directories in linux
ANSWER
    sbin are binary files only executable by users with administrative or elevated privileges
    or admin/root user while bin are binary files executable by any user

3) etc = contains configuration files
        /etc/shadow           = contains passwd of users
        /etc/passwd           = contains users imformation
        /etc/ssh/sshd_config  = ssh configuration details - determines if someone will use an ssh key or passwd

4) tmp = contains temporal files
         if you want to create some temporally files, this is where to create

5) opt = where software and packages are install
          install and download all packages/software in this directory

6) lib = library files
          put all library files here

7) var = contains dynamic files
          /var/log/messages  
   this contains dynamic files like log, what ever is happening in your server is recorded in the log file
e.g if you are unable to access your your server , there are some files e.g var/log/messages that you can go there to check

8) proc = contains information about our server, the hardware component
          meminfo
          cpuinfo
 

SIMPLE/BASIC LINUX COMMANDS
===========================

Run task/wprkload using commands
if we don't want to use commands we can use GUI
if you are using GUI , you are going to be paid something like [$30k-$60k]
but with the CLI , you are to be automating task for your client 
with this you will be paid like $100k upward 

we know that a directory/folder is a container that contains files
we have a new client = atango

You are given anew ticket to carry out task for ur client

TICKET 001
----------
       create work directories for atango
they want you to create a directory called
       1) devops
       2) dev/maven/git/aws/nexus/java     


CREATING, NAVIGATING AND MANAGING DIRECTORIES
=============================================

The first command is

       mkdir =  will creates a directory

if you create a wrong directory , you can delete the directory with
     rmdir = this command will deletes an empty directory(no content)

if the directory has content, we delete it with
      rm -rf - deletes a directory with content

now if i want to navigate from one directory to another, the command is
         cd

to know my present working directroy, the command is 
          pwd

listing the content of a directory, the command is 
          ls

Run a command mkdir -v directiryname
where -v = verbose mode

DEMO
---
    illustrate series of directory creations and demonstrations

To create a directory in this formate, dev/maven/git/was/nexus/java,  
we need to add -p , where -p stands for creating both the parent and child directory
i.e 
    mkdir -p directories or mkdir -vp directories

when you create a directory like this and run the command 'ls' , you only see the parent
directory, to see all the directories, we will run a command call the 
   tree - command
when we do this, the system will tell us that command not found,
here we can install the tree command using the a package manager called 'yum' , but to execute
this command, you must have root privileges/admin by using sudo, do not forget that when you use 
sudo, it permits you to switch or run commands as another user
so to install the tree command, run

         sudo yum install tree
DEMO
----
    how to install the tree command and use it to list the directories
deletes some created directories and do more demonstrations

LET US SEE HOW WE CAN NAVIGATE DIRECTORIES 
------------------------------------------
We navigate directories by using the cd command

DEMO
----
    demonstrate how we can move from one directory to another,
demonstrate how to navogate directories as dev/maven/git/was/nexus/java
i.e
---
    cd ..
    cd ../..
    cd ../../..
    cd ../../../..        
    cd ../../../../..

you may have to switch from one directory to another so please take note

if i do ls pwd = it will list the content of my present working directory
le dev = list the content in the dev directory
ls /home = list the content of the /home directory
le /dev = list the content of the /dev home director
