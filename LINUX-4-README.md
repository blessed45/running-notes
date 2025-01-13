#  **<span style="color:green">Prof Atanga.</span>**
### **<span style="color:green">Contacts: +237 652 177 151<br> WebSite : <http://solavisetech.com/></span>**
### **Email: ndecalamba@gmail.com**

LINUX 4
=======                   

  SYSTEM MANAGEMENT COMMANDS 
  ==========================
 
To know who is connected to ur server and at what time the user got connected and where the user is connecting from[ipaddress], we use the 'who' command.
                     
                        who
 

                 username              date      time    ip-address(where)
               ec2-user pts/0        2023-06-24  10:30    (129.0.226.22)
               ec2-user pts/1        2023-06-24  11:18    (129.0.226.22)
               ec2-user pts/2        2023-06-24  11:44    (129.0.226.22)
               atango   pts/3        2023-06-24  12:21     (129.0.226.22)

DEMO
-
    - Diagramatical illustration of users connected to a server and performing task
    - assign password to a user in your system and ask users to connect to it and
    - run the 'who' command and expain for more clearity

we also have other commands like;


               wc = the word count command

 If you want to know if a user connected to the server is doing some work or not; we use the 'w' 
command
              w  = tells u how long ur server has been up and running, who is logged in and 
                   if the person is doing some work or not

To see/know the list of all users connected to the server, run the command;
           
               users 

This will list out a compact list of all users connected to the server           

DEMO
-
     Run all the commands bellow

             whereis = gives you where a command is found in your server 

             df -h = tells you hw much storage you have and hw much you are consuming

             du  -h = will tells you how much storage you have consume      

             date = use to check the date

             date -s "date, time" = set the date of the server

             sudo timedatectl list-timezone = will list all the time zones

             sudo timedatectl set-timezone timezone = will set time zone

             sudo hostname  = wil show your hostname

             sudo hostname newname = will change you hostname

             sudo hostnamectl set-hostname newname = sets the server hostname perminently

             ifconfig (or) hostname -i (or) ip -a  =  will display the private ipaddress of your server
             curl ifconfig.co  


QUESTION
-
         Explain you experience with linux systems

ANSWER
-
       My experience with linux systems/servers include;

       - running workload using the 
           GUI or CLI
       
       - managing files using;
           1) touch command to create files
           2) vi command to modify files
           3) ls command to list content of directories
           4) umask command to set file permissions
           5) chmod command to set file permissions
           6) find command to fine files
           7) grep command to sort pattens from s file
           8) sort command to rearrange a file in alphabetical order
           9) sed command to replace/change content of a file
          10) echo command to print content in a file
          11) cp command to copy a file
          12) mv command to move a file
          13) cut command to cut portion of a file
          14) pipe command to enable the output of a command to become the input of another
          15) ln -s command to create soft link of a file           
          16) awk command to extract portion of a file 
          17) cat command to read content of a file
          18) > command to redirect content to a file
          19) >> command to apend content to a file
          20) ln command to create hard link of a file 
          21) rm command to remove a file
          22) cd command to navigate directories
          23) mkdir command to create a directory

       - managing users using;
           1) adduser command to add user to the system
           2) userdel command to delete a user
           3) usermod command to modify a user
           4) chage command to to change the default configuration of a user
           5) groupadd add a group to the system
           6) passwd command to assign a password to a user
           7) passwd -l command to lock a user's password
           8) gpasswd command to delete user from a secondary group
           9) groupdel command to delte a group    

      - managing and monitoring the system using;
           1) df -h  command to know hw much storage the system have and hw much has been consummed
           2) du -h command to know how much storage the system has comsummed     
           3) sudo hostname newname = command to change hostname
           4) sudo hostnamectl set-hostname newname = to set new hostname
           5) date command = to check system date
           6) sudo timedatectl set-timedate [date time] = command to set date and time
           7) sudo timedatectl list-timezone = command to list tme zone
           8) sudo timedatectl set-timezone timezone = command to set time zone
           9) who command = to know who is connected to the system
          10) w command = to know if users connected to the server are doing some work or not
          11) free command = to know the total memory of the system, how much is used and/or free
          12) whoami command = to know who you are

      - managing processes
           1) top command
           2) ps -ef command
           3) jobs command
           4) kill command
           5) bg command     
           6) fg command
      
     - managing packages
           1) wget command
           2) yum command / RHLE/Amazon 2/centOs
           3) rpm command
           4) apt / ubuntu/debian
           5) npm / node
           6) Chocolatey/choco / windows

     - managing services

          1) systemctl start/stop/enable/status/disable

           e.g
            systemctl start sshd
            serivce sshd start
  
     - security management    
          1) passwd command
          2) selinux
          3) firewale 


PACKAGE MANAGEMENT 
==================

Here we download packages and/or softwares to ease our task
download the following packages

    ssh client: mobaxterm, puTTY, gitbash
    text editor: sublime-text, brackets, vs-code, notepad++
    study platforms: zoom, telegram, whatsApp desktop

these softwares will make your computer to give you the study experience you need

Package management is a big deal when we are trying to automate automation
in linux we have some text editors such as 
    vim, nano,
some these editors are packages that need  to be install in our server
we can use these text editors to modify our files

For us to install a package, we use package managers
examles of package managers include;
    yum/dnf    = package managers for redhat/centOS
    rpm        = general package manager for redhat systems
    chocolatey = package manager for windows
    apt        = package manager for Debian/Ubuntu 
 
Now in aws, we have created a redhat server, so can install our packages 
Note that when you install packages, it can do some changes in you server
let me ask you this question, should any user be able to install packages in the server?
the answer is NO, so to install packages, you need sudo access
i.e 
          sudo yum install package/packages

To auto approve the process, use the -y flag at the end
i.e 
         sudo yum install package/packages -y 

After we install a package and no longer need it again, we can delete it;
   
          sudo yum/dnf remove package    

To download packages from the internet, we use the ;
       
          wget = non interactive network downloader

DEMO
-
     - install packages
     - install wget and downoad a package e.g apache maven

In our last class when we talk the linux file structure, we saw that packages should be installed
in the opt directory, so the recommended directory for us to always download packages should be the 
opt directory, everything in the opt directory is oen by the root user so to install any package there,
root access id required
 
We are explaining the fack that when it comes to linux, you experince is managing packages
and we can also manage process as well

DEMO
-
    - diagramatical illustrating of users connected to a server ding different tasks , like
      five of them, managingfiles, managingpackages, managingsystem, managingservice, 
      managingprocess, backingup data etc

Anything that we do in the server is a process in linux thus the need for process management

PROCESS MANAGEMENT
-

             FileMGT
             UserMGT
             ProcessMGT
             SecurityMGT
             PackageMGT
             ServiceMGT
             SystemMGT
             Monitoring
             dbBackup

Tasks are processes running in the system
we have commands here like;

       top command

DEMO
-
     run the top command and explain while laying emphasis on load average
     be remimded of the fact that load average is on 1

IQ
-
   what is load average in linux
ANSWER
      the load average tells you how much load a system is carrying

To make sure that your system don't break, load average should be highly considered,
this is because, when the load average is high, the server can come down or will run
very slowly

    
Every task/workload we do on the linux server is a process, by such;
processmgt is very important,
its through processmgt that we can know and correct the state at which our server is 
running, processes that have no use in the server can slow down the server and make 
it to malfunction or slow down, e.g of such processes are the zombie processes or the process with z in STAT column


the 'ps', 'ps -ef', 'ps -f', command will display the state of all processes in ur server

NOTE: Every process has an ID known as the process ID [PID]

if we find out that there is a process in the server that is not useful, we can kill the process
 by using the 'kill PID' command and the process will be killed

i.e

kill PID = kills a process with said ID

HOW TO FIND IF A PROCESS IS NO LONGER USEFUL BEFORE DELETING
=============================================================

We run the command;
'ps - aux' = this will display the content of processes running in the server, look for the column with 
letter 'Z' and kill the process by using the PID as shown above

or better still, we can run the command

ps -aux | grep Z = this command will display all processes that are in the zombie state. showing the process
 id [PID] , parent process id [PPID] and the command that was use to start the process  

HOW TO KILL A zombie PROCESS
============================
We run the command;   

'kill PID' = this will eliminate the zombie process and thus speeds up ur server

To forcefully kill the process; run,

'kill -9 PID' = it will forcefully delete the process if the later did not work 

Istall apache httpd and check if the servive is running

         ps -ef | grep httpd
         
DEMO
-
    - do illustrate more examples
    
                 
SERVICE MANAGEMENT
=================
      
      service servicename arguements
      service servivename start/stop/status/enable/disable/restart
      
      systemctl arguements servicename
      systemctl start/stop/status/enable/disable/restart servicename

DEMO
-
     start some services, check their status

Q
Exlain your expereince with linux systems
==========================================

My experience with linux systems include;
    1) deploying, povisioning and creating linux servers in AWS cloud,
       connect to servers using - ssh protocol

    2) configuring, optimising, commissioning, decommissioning and securing linux servers

    3) running workloads in linux servers/systems using;
            GUI
            CLI
            SCRIPTS
   
     examples of workload/tasks executed include

             FileMGT
             UserMGT
             ProcessMGT
             SecurityMGT
             PackageMGT
             ServiceMGT
             SystemMGT
             Monitiring
             dbBackup

We commission a server by installing the application software in the server
and decommissioning is uninstalling the software 

As we move on with the course, we will see how to automate task using scripts and cron table

with cron tables we will see how to schedule and automate tasks
we say something like 
 1) Backup all databases every midnight
 2) desplay the latest version of the application every sunday at midnight
 3) optimise our appservers every month on the 28th day
      like ; yum update -y && yum upgrade -y
 4) monitor system resources and sent send alert using threshold every minute
      like ; if cpu/mem usage exceed 80% sent email df -h = cpu

these are the kind of tasks we are going to be seeing through out the course

  ARCHIVE/DATA BACKUP COMMANDS

To backup database, we either copy the file or we zip or tar the file
i.e
       zip   =  package and compress(archive) files
       unzip = Extract compressed files in zip archive
       tar   = use to archive a directory/file

DEMO
-
     - vim into a file with much content and zip the file
     - install the zip package
     - zip file to a file called filename.zip
     i.e
         zip newfilename.zip filename
    
     - compare the volume of storage consummed by the file and the zip file 
Note when you zip a file, there is no need to keep the original copy, so you delete it,
because if the file still exist, you will not be able to unzip the file

to tar a file, we run;

      tar -cvf newfilename.tar.gz filename  =  compress a file
      
      tar -xvf filename.tar.gz              =  extract compressed *.tar.gz file 

DEMO
-
     ceate a tar file and extract the file


You have a blocker, how will you resolve it
==============================================
1) check company's documentation--- running/pdf notes , videos
2) contact team members
3) use AI platforms [google, youtube, chatGPT
4)communities  

We run different tasks on our servers to manage applications
workload executed in application managenment
===========================================================

   1) usermgt
   2) files/codes = filemgt
   3) securitymgt
   4) processmgt
   5) systemmgt
   6) packagemgt      

HOW TO EXECUTE WORKLOAD
========================    
    
    1) GUI = graphical user interface = less than $90k
    2) CLI = command line interface   = more than $150k 
    3) SCRIPTS ( a sctipt is a reusable code/file) = $200k 

So far we ahve executed commands and commands are going to help you achieve 
your tasks with relative ease

Now lets look on some other commands

OTHER COMMANDS
===============

DEMO
-
    connect to a server and demo a couple of users connected to 
    the server from their systems and outline what they need to 
    connect to the server, 

For users to connect to a server, there is a process called sshd  
service must be running before you can connect to the server

e.g
    somebody tells you that he/she is unable to log into the server 
    with all credentials correct, expalin what could be the problem

           1) check if the user is running the ssh command correectly
                     
                      ssh username@ipadderss

           2) check if ssh port 22 is open on the firewall/security group

           3) check if the server is up and running  
                  
                 ping the server

           4) check if the sshd service is running, if not start the service 

              sudo systemctl status sshd = to check the service
                
              sudo systemctl start sshd = to start the service 

Lets now look at some other commands
1) clear = this command will clear the terminal screen

2)   cal  = this command is use to check/set the calender on the server

e.g       
        cal june 2023 = will give you the calenda of june 2023
        cal july 1982 = will give you the calenda of that year

if you want to know the day that you were born in the week; run the cal command

3) wget  = this is a none interactive network downloader user to download files
           from the internet

   e.g  
       there is a time that you want to download a package, the system interacts with you;
  i.e
      ask you if what you want to do is ok by you,
That process of the system asking if you are ok or not is known as interaction,
here we say the system is interacting with you

We can still as well ignore the interaction by using the -y flag

WE HAVE LEARN THAT IF WE WANT TO DOWNLOAD ANYTHING, WE SHOULD DO IT IN THE [opt] DIRECTORY
-
i.e = cd into the 'opt' directory and download what u want to download from the internet there 


4) echo = this command prints what ever you type

5) tee  = this command is use to store and view the output of any command at the time   

    e.g
        run on the terminal,
                            echo "at 360k a year i am rich"
                            echo "with DevOps i'm a millionaire"        
        demo the echo message and re-direct to a file call rich
        cat the file rich, pipe and tee newfilename

6) history = this command displays the ecently executed commands
           = all the commands that we have been ruuning are stored here

7) watch = this command is use periodically 
          - with this command you watch what is happening to youe file system
            or your memory
       
               watch df -h  = checks file system
               watch free -m  = to check your memory  
     
Take note; this command is very good for file monitoring

8) ping = this command sents ICMP ECHO_REQUEST to network host,
          - checks for network connectivity
         e.g
             i have a database server i want to check, are you alive? 

9) telnet    = a server uses ports and protocols,
               the number of ports in a server/system/computer are 0-65535 ports[addresses] by default
               So any server that you create has these number of ports/addresses 
           e.g
               if somebody tell you he/she can't access his/her server, you can check if the required port
               that the server is running is open

                               telnet server-ipaddress portnumber 



10) reboot =   this command will reboot the server and it also need sudo access

11) restart =  this command is use to restart the server and it requires sudo access,
                take note that when you reboot/restart a server, the ipaddress of the
                server can change 

12) shutdown = this command is executed with sudo access
             - use to shutdown the system
             - you will find a warning while try to run the command

13) uname   = this command will describ your system
           
             uname -a = tell you all information about your server

             cat /etc/*release  = tell you detailed information about your server

             cat /etc/*os*   = tell you detailed information about your server


14) netstat   = remember the number of ports in a server/system/computer are 0-65536 ports[addresses] by default
                       So any server that you create has these number of ports/addresse
                     - with the help of this command i can know how many ports that are in use
                     - let assum that we want to install ngnix, and nginx is using port 80/443,
                       so for you to know the ports that are in use before installing an application 
                       that runs on a particular port number, we use netstat command to check if the
                       port is in use or not, this is because if that port is already in use, that package
                       will not be able to run
   NOTE 
       if you run netstat and the system tell you command not found, you can install the command by running
                            
                  sudo yum install net-tools -y = will install netstat command
  
Now we can check the ports by running,

                    netstat -tulpn  = will list all the ports in use

                    t = tcp
                    u = udp
                    l = listening 
                    p = port
                    n = number

     protocols        ports/address
       ssh                 22
       http                80
       https               443
       nfs                 2089
       rdp                 3089 
       smtp                25/465/587
       tomcat              8080
       jenkins             8080
   
 15) man = diplays the on-line manual type
          - tells you everthing about what a command does
      e.g
          run,  
              man ls

16) help  =  helps you on how to use a command

17) info = helps you with information about a command
          - make sure you install the info command before executing

18) whatis  = diplaces the manual page of a command

19) service = it will give the status of service

             service sshd start
             systemctl start sshd

20) systemctl list-unit-files   =  it will list all services

21) uptime  = tells how long a server has been up and running 

When it comes to linux commands , i think we have come to the end of all
that is required you know as far as this course is concern

We have come to the end of the first MODULE
Our next MODULE will be SCRIPTING
In the MODULE, we will be learning how tasks are being automated to 
a higher level
