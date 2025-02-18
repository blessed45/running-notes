#  **<span style="color:green">Prof Atanga.</span>**
### **<span style="color:green">Contacts: +237 652 177 151<br> WebSite : <http://solavisetech.com/></span>**
### **Email: ndecalamba@gmail.com**

LINUX 2
=======
                            
                
In our last class we started seeing what is linux and how our job looks like as a devOps engineer
so today we will be entrying to our fisrt module which is a very important module, so take note

As a devOps engineer, you will be working with your team to;
===========================================================

develop: Applications

Test: Applications

Build: Applications

Review and qualiry: Applications

Secure: Applications

Deploy: Applications

Access: Applications

Maintain: Aapllications

Manage and monitor: Applications

All these jobs are done by using automated computerise technologies

e.g 
    if you go to any credit union or bank, how do you access your account on the internet?
    you can go to the bank's website  
    you can be ask to enter your;
        
        login information
        user name
        card number  
    
    to access your account, you need some credentials and all those credentials are jobs done by devOps engineers
    i.e all the login information or registrations in banks are done by devOps engineers, so as a devOPs engineer,
    you will work with your team to develop, test, builded, review, secure, deploy, access, maintain, manage and minitor
    applications
 
As we said, all this is done by using computerise automated solutions, so generally, if we use computerised solutions, this means
computers are involve 
 The big question here now is what types of computers are involve?

PERSONAL COMPUTERS
-
        
        -laptops, phones, tablets, watches
        - memory = 4gb, 16gb, 32gm, 64gb
        - cost = $400-$2,000  

PROFESSIONAL COMPUTERS
-
        
        -workstations, laptops, 
        - memory = 8gb----256gb
        - cost = $700-$20,000

ENTERPRISE COMPUTERS
-
          
          -servers
          - memory = 128gb----4000gb
          - cost = $2,000-$200,000

But our job is to help companies using computerise solusions either by going to the market to buy servers and come and install or we use cloud service providers (CSP)
So today, most companies move to the cloud service providers (CSP) for servers , these companies have a lot of computers that they have configure then together, network them and just waiting for companies


CSP = cloud service provider
e.g
   AWS, AZURE, GOOGLE, ALI BABA, IBM etc

Let us look at

BSP - FINTECH: Banking service provider
what we can do in a bank
             
             create account, tranfer money, exchange, withdrawal, cash deposit,
             cheque deposit, loan, overdraft

for this work to be done, a bank like Ecobank will need to imploy like 900 workers 
to be executing this job and most of them do this job manually, 

Now devOps engineers develop, test, build, qualify, deploy, manage and monitor applications
e.g eletronically you can do anything now without neccesarilly going to the site,
       
       you can now create an acoount online, buy online, there a lot of things that we do now online,
       here you are ask just for neccesary credentials, like
               
               username 
               email
               password 
               card number
               phone number
               postal code, etc

Let us noe see why DevOps engineers are being paid high,
This is because their main job is helping companies to make a lot of money
they continuesliy intergrate and deploy using automated solusions not manually

what banks do now is that, they fire more of thier manual workers and imploying devOPs engineers.
This is because the job that 200 worker can do manually in a company can be executed by at most 4 devOps
engineers, so you see now that companies pay them high and yet still save more money since they have less workers

DEMO
-
    Any mathematical illustration of how a company make moere money by employing few devOps engineers and sacking
    more manual workers

At this juncture, we will create another linux server to those are still unable to create a server 

 server
        name = dbserver
        ip-address      = ?
        username        = ec2-user
        password        = ?
        ssh private-key = atango

we learn in our last class that when we create a server, it come with the ip-address and a user called ec2-user
So to access an ec2 instance/server we need the above credentials, with all that put in place, we can now connect 
to our server through ssh protocol

            ssh -i public-key username@serverip-address   # when using a key pair
            
            ssh username@serverip-address                 # when using password 
DEMO
-
    create a new server and connect to it using different methods

we run this course for like 5-7 months because we want you guys to know hardcore IT from end - end
Don't worry, as we move on, the course will be deply to you simlessly ,
So you see, in two minutes, we have launch a server,
this is what a company does for 1million CFA 

in our last class we started looking at some few commands, so we will proceed with that from here

DEMO
-
    - revise the pass command that was treated in the last class,
    - illustrate with examples and create more files and directores
    - do it to the undertanding of every one

These are commands that will help use to navigate a directory

Now let us look at commands to manage files


 FILE MANAGEMENT COMMANDS
===========================

The command to create a file is called the 'touch' command

       touch = creates a file

TICKET 002
-
Create the following files
      
      list.txt               
      hello.py
      greet.sh

OPTIONS 1
-
     
     touch list.txt
     touch hello.py
     touch greet.sh

As a devOps engineer, your job is to automate task, though we can create these files one after another,
if you do that , you are a junior engineer, as a devOps engineer, you must always take automation to 
another level, we can be using GUI as is we are typist, even when we use CLI, we must automate.
The second option will automate the task

OPTION 2
-
        
        touch list.txt hello.py greet.sh

Now can see that just with one command, all the files have been created, this what we called automation.

We have seen how we can create a file but all the files that we created are empty files,
we will now see how we can create files and add content

let say you first day at work , you are assign a ticket,

  Creat a file (list.txt) and add content      

1)emmanuel
2)ernest
3)vitalis
4)paul
5)john

Please take note about what we are about to do now, because when ever we reach at juncture, most foxs
get confuse, so i will expert some of you to get confuse but just pay kind attention, you will understand 
all what is needed of you here, the course will be deployed in such a way that every body will have a full
mastering of it,

Here,
     we will look at a new command called 'vi'

This "vi' command has a command mode and an insert mode

you start accessing the file in command mode
when you 'vi' you are in command mode, in command mode, you cannot modify or add content
to start modification or addition of content, press letter 'i' on your keyboard,
when you do this, it takes you to the 'insert' mode and to get out of the 'insert' mode back to 
the command mode, press the 'Esc' key on you keyboard, 
Now in command mode, for you to save and quite, you press ':wq!' enter  

If you want to add modify the file , you still 'vi' into the file, press the 'i' to enter insert mode,
the 'Esc' key to go back to the insert mode, then ':wq!' to save and quite

If you make a mistake with the file and to quite without saving, you go back to command mode and press
':q!'  

There is also a shortcut to save and quit
do a quick double press on the 'shift+z' key to save and quit = press+hold
 i.e
     press the shift botton and hold, then double click on letter z

DEMO
-
    illustrate a couple of examples on this

When it comes to modifying files, we can use text editors
e.g 
   of test editors thst can be use to modify files include

in windows
          sublime text
          notepad++
          braket
          vs code
          atom
          eclips          

when developers are writing codes, they use text editors for coding and 
later copy and paste, they do this to be sure before deployment, they don't 
get directly into vi

We have seen how to create a file and add content and modify a file

Let us now see how we can read content in a file

to read the content of a file, the command to use for that purpose is the 

  'cat' = this command will read or display the content of a file

so to do that we run the command as folow

    cat filename

If we want to display the content of a file with all it's lines numbered, you pass the -n ,

    cat -n filename  

There some other commands that can be use to display the content of files, such as the;

        head = will displays the first 10 lines of the file
                    
                        head filename 
for the last 10 lines
         
         tail = will displays the last 10 lines of a file

                        tail filename

If you want to get the first 5 lines or last 5 lines , run

                        head -5 filename
                        tail -5 filename

We also have the less and the more commands that are use to display files

                less filename
                more filename

when you use the less or more command, press q to get out of the file

For backup, we create a copy of the file  

BACKUP FILES
------------
The command to create a copy of a file is 

  cp = creates another copy of your file
        
          cp filename newfilename 

We have a command used to rename files, this command is the;

      mv = rename and/relocate files

      mv filename newfilename

When it comes to file management, we can create files, add content to files, move files from 
one directory to another

We can also;

- delete files
    
           rm filename = will deletes a file

           wc filename = word count command

           wc -l filename = displays number of lines in a file 

if you want to create a link to a file, the command is;

           ln filename newfilename = creates a hard link of the file

hard links are like copy of the file, there is also a soft link called a symbolic link
to create a symbolic link, run

            ln -s filename newfilename  = creates symbolic links

DEMO
-
     - Create some hard and soft links of files and demonstrate the differences             
     - differentiate between hard and symbolic link

FILE MANAGEMENT COMMANDS
------------------------

  touch                      = creates a file
  vi                         = create a file /or modify/edit a file
  cat/head/tail/less/more    = permits you read a file
  wc                         = word count command
  cp                         = copy a file / create backups
  ln                         = creates symbolic links
  mv                         = re-name or migrate a file or directory


There are some other file management commands that we need to take note of
when we create a file, it has what is called a file permission
e.g
     d rwx r-x r-x. 3 ec2-user ec2-user 17 Jun 19 17:33 dev
     -rw-r--r--. 2 ec2-user ec2-user  1 Jun 19 14:33 mytest
     -rw-r--r--. 2 ec2-user ec2-user  1 Jun 19 14:33 test      
     l rwx rwx rwx. 1 ec2-user ec2-user  8 Jun 20 18:29 test.txt -> test.txt



     1       2      3    4        5        6           7         8
     d  rwxr-xr-x.  3  ec2-user  ec2-user  17  Jun 19  17:33    dev
     -  rw-r--r--.  2  ec2-user  ec2-user  1   Jun 19  14:33    mytest
     -  rw-r--r--.  2  ec2-user  ec2-user  1   Jun 19  14:33    test      
     l  rwxrwxrwx.  1  ec2-user  ec2-user  8   Jun 20  18:29    test.txt -> test.txt

In this file structure, we have what is called the field of the file or directory

FIELDS FOR FILES
=================

       r = read
       w = write
       x = execute

       1) type  =  here;    [- = stands for a file,  d = stands for a directory and l = stands for a symbolic link]
       2) permissions       [ rwx,    r-w, r-x ]  
       3) number of links
       4) owner
       5) Group owener
       6) size of the file in bytes
       7) date and time of creation
       8) file name and directory name 
        

Why do you think the prmission of a file is very important?
we have three categories of permissions, namely 
     the, 
          - rwx = read write execute
          - r-w = read write
          - r   = read
By default, the first file permission belongs to the owner
i.e
    rwx = owned by owner
    r-w = owned by group 
    r   = owned others

File permission is a key facture when it comes to security
so please take note about that

Now we are going to deal with a very important aspect as far as files and directories are concern,
This will be file security and permissions

  FILE SECURITY AND PERMISSION
  =============================
Generally we have three categories of individuals that can access a file, they are;

        - owner
        - groupowner
        - others
Since we have three categories of individuals that can access a file, these files are are also access in different
levels, the levels in which we can access a file include;

          you can read a file
          you can write or modify a file
          you can execute a file
i.e
          - read
          - write
          - execute

The write access is the superior access to a file, this is because when you have a write access to a file, you are 
able to modify the file while others can not, 
You come to discover that with the executable access you can use the file for automation or to run some other commands

The accesses are assined some numbers by default,
i.e          
          r - read    = 4  
          w - write   = 2
          x - execute = 1

Take note that we have a directory that we have created, and a file
I that directory and files, we have;

     drwxr-xr-x. 3 ec2-user ec2-user 17 Jun 19 17:33 dev
     -rw-r--r--. 2 ec2-user ec2-user  1 Jun 19 14:33 mytes

look closely at the permisions of the directory and that of the file
you will find out that they have different permissions
 i.e
     d rwx r-x r-x. 
     - rw -r-- r--

From the above default values of permissions, we can now say 

                  owner        groupowner       others       default permission
directory         rwx = 7      r-x = 5         r-x = 5             755
file               rw = 6      r-- = 4         r-- = 4             644

all what we have done here is known as the default permissions of files
Note that these default values can be changed

if we want to assign full permision to a file, it means that any body in the os can read and write in the file
i.e
   from what we have above, the file will have a permission
            
             0666

And for a directory, it means any body in the os can read , write and execute
and from the our default values above , we will have a full perssion as;
            
             0777

Now we have seen the full permissions for directories and files and the default values,
The difference between the full permission and the defaul permision is called the;

           the UMASK value      
i.e
                      file     directory        
   full permisions    0666      0777    
   default perm.      0644      0755
                     ------    ------ 
    umask value       0022      0022 

So from our calculation, we have all seen that the umaxk value is;

                umask  =  0022

Therefore, the default umask for a root user is 0022 and that of a normal user is 0002
Take note only about this two values because all those calculations were just to show
you how the umask value is derive

IQ
-
   What is the default umask value of the root user and a normal user

NOTE
-
    The umask value is what is used to determine the default permissions of a file or directory
    during creation 

DEMO
-
    illustrate some few files and directories creation and show what happens as far as file 
    permision is concern

We have seen that in all files and directories created, they have 0644 and 0755 respectedly;

Now if you are given a task to create files with permisions 0600, this means that only the oner 
of the file can read and write in the file, the group can not read nor write and even others,
With such a file, what do you think could be the umask value?

we all know that for all files that we create, they have full permissions or custom permission,
          
              0666

and now, we are expected to create a file with custom permissions 0600    
This means that the umask value of this kind of file is;

   default full permisions           0666
   required permission             - 0600
                                   -------
   umask                             0066

Set a custom umask value to ensure that all files created should carry 600 permissions

NOTE
-
      to check the umask value , just run the command  =   umask
DEMO
-
    set the required umask value, use the command

              umask [required umask valur]
  e.g
  -
            umask 0066 
   
   After doing this, created a file with thw 'touch' command and illustrate the file permission,
   if it has change or not

I will like us to know that, we will not be using the umask command to change permissions of files
as we move ahead, there is a simpler command that we will be using know as the;

                chmod = this command is use to change file permissions
i.e
-
                chmod 600 filename = is same as setting the umask to 0066, before creating a file 
So take note

DEMO
-
    Create some files and directroies while changing their permissions with the chmod command
    Use created files to show how automation access is granted to group and others, illustrating
    the importance of why file permission is very important,
e.g
    like a person can be sacked from the office while he/has had control over a file and another person 
    has replace the he/she and the file now will be run by the new person, so the ownership has to be changed,
    
Changing owners of group are not done by normal users in the OS, so for you to change the ownership of a file,
you must posses elivated priveleges or root access, or sudo access
   so for you to change the ownership of a file, you need sudo access and take note that you can not change the
   ownership of a user that doesn't exit in the system.

               sudo chown

To change the group owner also, you can run the command 

               sudo chgrp

We can change the owner and the groupowner at the same time, since our job is to automate task, we can run;

               sudo  chown ownername:grpowner

DEMO
-
     illustrate how ownership is being changed for owner and groupowner in a directory or file
      demonstrate couple of examples to the understanding of foxes
