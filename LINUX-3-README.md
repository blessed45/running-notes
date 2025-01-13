#  **<span style="color:green">Prof Atanga.</span>**
### **<span style="color:green">Contacts: +237 652 177 151<br> WebSite : <http://solavisetech.com/></span>**
### **Email: ndecalamba@gmail.com**

LINUX 3 
=======

As we know, as DevOps engineers, we work hand in hand with our team to;
            
        develop
        test
        build
        reviw and qualify 
        secure
        deploy
        maintain
        manage and monitor
 software and applications using computerise solutions

As a DevOps engineer, the only task that you are not directly involve is the first one (development)
and software engineer, the rest we are directly involve

Here are some examples of jobs that we will be doing as DevOps engineers

  DevOps engineer
  DevSecOps engineer
  cloud engineer and/or
  AWS cloud engineer
  platform engineer
  Infrastructure engineer
  Kubenetes engineer or
  Sr. IT recruiter
  IT project manager
  Scrum master
  Build and release engineer
  SRE

DEMO
-
     illustrate some few platforms 
     demonstrate with diagrams how users are able to connect to the server while
     performing task.
e,g  
   linux, windows etc
If you can work only one platform or several platforms, performing task/workload such as
      
          - troubleshooting and fixing problems resulting from platform failures
          - enhance the platform by doing some, upgrates, updates, patches
          - securing the platform
by doing all these you are platform engineer

In our last class we look at some certain commands,

i.e
     umask
     chmod
     chown
     chgrp  

DEMO
-
    connect to created server and do some revision
    continue with more commands demoanstrations
    'ls' into a file that has more content and demo the 'grep' command 

In linux, there is a command use to extract pattens from files and that command is known as the;
     
          grep  =  sort pattens from files
DEMO
-
    demonstrate, with a file that have repaeted names, some with upper case letters and illustrate
    how the grep commands works and explain the case sensitiviy in linux

To ignore the case sensitivity, run the command with the -i flag

               grep -i = will ignore case sensitivity



The next command we will look at is the pipe '|' command

The pipe enables the output of a command to be the input of another command or 
the next command

please take note

IQ
-
 a) what do you undertand by the grep command in linux

ANSWER
-
the grep command is used to extract pattens from files
 
b) explain the difference between the grep and the pipe commands

DEMO
-
    - lllustrate how a file can be read and the output stored temporally by the pipe command and
      extract some file content using the grep command
    - demonstrate diagramatically for better understanding
    - use a watertank , pipe and house deployent demo  
    - illustrate cat /etc/passwd

There is a command that is use to re-arrange a file in alphabetical order and that command is known as the,
the sort command
                  
                 sort = re-arrange the file in alphabetical order
DEMO
-
     - run the 'sort' command to show how it re-arranges the file in alphabetical order
     - also run the cat /etc/passwd | grep (anyname) | sort
     - run the grep command while ignoring the case sensitivity [grep -i]

There are other commands such as ;

      find = search for files and directories

here we run the commads as follw

    find  (where you want to search for the file)  filename 
    find /home/ec2-user filename
where /home/ec2-user is the home of ec2-user, that's whee we want to search for the file
the home of ec2-user can still be represented by ~

               find ~ -name filename
               find / -name filename  = / is the root directory

To seacrh for file in your present working directory 'pwd'
you run ;
               find . -name filename
DEMO
     run some few examples demonstrating the above commands

We can also set the date of our server using the 'date' command 

               date = shows you the date of your server

               sudo date -s  = sets the date of you server

you will realise that these servers we are working on will be use to schedule jobs, let us assum that
we have schedule that a process in our server should backup data every 12 midtnight, should anyone be able to 
change the date? The answer is NO , so that is why you must be duty authorise before setting the date od a server,
so you have to run the command as the root user as follow

                  sudo date -s "date, time"

                  sudo date -s "20 Jan 2024 9:00:00"
 
DEMO
-
    set the date and time of the server for better understanding, do it first as normal
    user and see the error then as root user

We can also change change the timezone by running the command
    
         sudo timedatectl list-timezones

after running the command copy your prefered timezome and run it as follow to set the timezone

               sudo timedatectl set-timezone timezone

               sudo timedatectl set-timezone Africa/Douala


This is user management, so take note
The big question here is who to do what and at what time in the server

In linux, we have a normal user and the root user

The root user is a the admininistrator/admin/super in the server that can run all commands and task
unrestricted

In linux, the root user is called root
when you create a linux server, the root user is created by the system when a server is launched/created

We also have normal users
   The normal user is created by the root/admin user

If we want to create a user in our server, the command is very simple, the command is;

               adduser
               useradd
But for us to creat this user account, we need root access/ admin access
i.e
     sudo adduser username
     sudo useradd username

For e.g you are given a task, create users accounts for emma and ernesrt verify

Remember when we run commands with sudo, we are running the command as the root user 
 
DEMO
-
    - create account for emma, start by doing without the sudoers access before applying
      it for better clearity
    - do more demonstrations
    - demo sudo -u ec2-user for normal user and sudo -u root for root user

Now to verify if the user was created or not, there is a file where when ever you create a user
in the system, the user imformation is stored there and is known as the  /etc/passwd, so if we
'cat' this file or grep for the name in the file or tail the file  
we will see if the user was created or not
i.e
     cat /etc/passwd  =  allows you to check for user information 
     grep username /etc/passwd
     tail -2 /etc/passwd

Or you check it in the /home directory with the 'ls' command 

DEMO
-
      'cd' into /etc, 'ls' and do some illustrations

When it comes to accessing files, we have the relativePath and the absolutePath

                relativePath  = starts from pwd
                absolutePath  = starts from the root directory (/)
DEMO
-
    
To assign or modify pass word for a user, we use the passwd command
i.e
           passwd = use to either assign or modify user's password

Note that, to change the password of a user, u must have root access

               sudo passwd usernsme

But to modify your own password, you don't need root access

To switch from user to another, we use the commnd 

               su

For e.g if you want to switch user as root, execute

              su - root
NOTE ,
-
      if you are connected to a server as a normal user and want to switch to another user,
      the system will ask you for the user's password
Don't bother, you are going to have a whole book when you start working that contains most
of these commands

So to switch to another user, use 'sudo'

      sudo su - username 

The root user run all commands without restrictions , so take note that it is not advisable
to be running task/workload in the system as a root user, for security reasons, always run task 
as normal user

DEMO
-
     - demo as root user and normal user

          $ = normal user
          # = root user
         
      - assign password to a user and use to illustrate some few examples
      - emphacise the login imformation given by the server during a failed
        log in
      - Switch to a user created and try to switch to root user 
      - illustrate the information given by the system
      - explain why you can not use sudo access as normal user to switch
        to root user,

As a normal user [created user] you can not switch to the root user or any other user, unless
you are given the previleges to do so, 
To do that, there is a file called the /etc/sudoers , so the admin user will vi into this file 
and add the the user's name whose previleges are to be elevated

GRANTING SUDOERS ACCESS
=======================

           sudo vi /etc/sudoers

when u modify the file, to save and quit press [:wq!] then [enter]

search for the sudoers line and insert the name

OR,
   Just run the command
  
     sudo echo "username ALL=(ALL) NOPASSWD:ALL" | sudo tee /etc/sudoers.d/username        

NOTE,
-
      by default, the ec2-user comes with sudoers access

DEMO
-
     - 'vi' into the sudoers file and grant sudo access to a created user
     - also run the second command to illustrate  

Note that it is preferable to copy the second command and keep it safe so as to
always copy and paste when ever you want to assign sudo previleges to a user 


   User management task/workload includes;

   - creating groups
   - creating user's account
   - assign password to users
   - add users to groups
   - modify user's account
   - delete a user
   - elevate user's privileges
   - re-set user's password
   - lock a user's password
   - unlock a user's password
   - set expiration date for user's account/password
   - assign task to users
   - grant and remove admin/sudo privileges

Creating user's account requires sudo/root privileges
We saw in our last class how we can assign sudo privileges to a user

Now let see how we can assign password to users
To do this, we all know that you must be authorise and we have already seen how to authorise a user
If you have sudo access, you can assign a password to a user
i.e
               sudo passwd username

the above command will permit you to assign a password to a user    

We can also create groups in the system and this also needs sudo access
i.e
               sudo groupadd groupname

         sudo groupadd group-A && sudo groupadd group-B && sudo groupadd group-c = task automation
                                  # you can use && or : to seperate the commands 

We can add users to groups
e,g
  a user's account is created and that user is an engineer, so, we have to add the user to the engineer's 
  group 
This is done by using the command known as 'usermod'
i.e
                sudo usermod -aG groupname username = add user to a secondary group
                sudo usermod -g groupname username = add a user to a primary group

the above command will add a user to a secondary group, secondary group because when a user is created in 
the system, the user comes with the user's home directory/users group

We can delete a user from the system and to do that you need sudo access 
this is done by the 'userdel' command
i.e
                sudo userdel username

note that this command will delete the user without the user's home dierctory

But if you want to delete a user with the user's /home directory, add the -r flag
i.e
               sudo userdel -r username

this will delete the user with the user's /home directory

Please take note of this command,
To delete a user's hone directory after the user have been deleted without the /home directory,
run the command;

                   sudo rm -rf /home/username

This will delete the user's home directory with relative ease

And to delete a user from a secondary group is what you should also take special note of.
To do that, run the command;

                  sudo gpasswd -d username groupname

Take note of the above command 

There is a file called /etc/group
So if you want to verify the number of groups existing, you cat the file
i.e
                  cat /etc/group

Now if you want to know a group that a user belongs to, there is a command called 'id'
run the command and it list all the groups that user belongs to
i.e
                 id username

DEMO
-
     illustrate series of examples

Elevate user's previlieges
For you to achieve this task, as we saw in our last class, we can;

                 sudo vi /etc/sudoers  
                 sudo visudo

either you vi in the file and modify it or you run the below commnd

                 sudo echo "username ALL=(ALL) NOPASSWD:ALL" | sudo tee /etc/sudoers.d/usernam
DEMO
-
     - demonstrate while explaining detailly for more understanding 
     - grant sudo access to some created users in the system or create new users and and assign 
       sudoers access to them
     - assign password to users 
     - switch from one user to another

Note at this juncture, when a user is granted root/sudo access, that user can perform 
tasks/workload as the root user, 
i.e
   the user has elevated privileges and can now run tasks/workloads like;
   assigning password to users and any other task done with those privileges by 
   passing the sudo flag 

DEMO
-
     switch to a user with elevated privileges and assign password to anothe user

To remove sudo access from users, vi into the /etc/sudoers file and modify the files
by deleting the user from the sudoers file

DEMO
-
     illustrate how to remove a user from the sudoers file

For example if someone is at work and not doing anything, what do you think we can do to that
type of a person? We can lock that person's account, and for us to do that, the command is;

                      sudo passwd -l username

to unlock back the account, we are going to run the command;

                      sudo passwd -uf username
                      sudo passwd -u username

To set expiring date for user's account/password
we all know that this are admin tasks, so sudo access is required
and the command is;

                     sudo chage username

DEMO
-
    illustrate while explaining all the parameters
    i.e
       minimum password age [0]:
       maximum password age [99999]:
       last password change (YYYY-MM-DD) [2023-08-31]:
       password expiration warning [7]: 10
       password inactive [-1]: 10
       Account Expiration Date (YYYY-MM-DD) [-1]:

So with this chage command, we can set some default value for a user

Now we have understood some basic user management commands

HOW CAN A USER ACCESS THE SERVER/EC2 INSTANCE EXTERNALLY USING PASSWORD
-
Take note of this, it's very important
 
For you to do that, the server must be configure such that it can be access externally
There two ways of doing that;

1) copy the follow two commands and paste;

                        sudo sed -i "/^[^#]*PasswordAuthentication[[:space:]]no/c\PasswordAuthentication yes" /etc/ssh/sshd_config

                         sudo service sshd restart
                         sudo systemctl restart sshd

                         

OR
-

2)   We vi into a file called (/etc/ssh/sshd_config) and change passwd authentication = NO to passwd authentication = YES
after that, save and quite

                           vi /etc/ssh/sshd_config

once you do that, restart the ssh service by running; 

                          sudo service sshd restart

this will finish confuring ur change

     Note that even with all credentials of a server;
i.e
      server ip-address
      username
      password 

You can not access the server externally, except it is the server has been configured
in such that it can be connected to externally

And note that when ever you do a change in the ssh service / configure a server, you
must restart the service, if you do not, the changes will not be executed by the server

I recomment for you to always use the first method of copying the two commnds and paste
because if you vi into that file and mess it up, you will not be able to log into that server 
again, either through ssh or password and/or externally
 
DENO
-
     - demonstrate by vi into the file, then run the command


At this point, i think we are done with user management commands and don't worry, the cousre will
be deploy in such a way that everbody will understand. 

From here we will be looking at commands to know who is connected to your system, what
they are doing and at what time they were connect, we are talking of commands that can be use to manage our system, known as system management commands or system resources management commands
