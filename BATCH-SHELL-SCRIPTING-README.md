Bash Shell Sripting
===================


DevOps/Cloud/SRE/DevSecOps/Build and release Engineering
Platform/Kubernetes/Infrastructure Engineering
========================================================

Automating IT processes/workloads with GUI/CLI and Scripting
=============================================================
Automating IT:
   processes
   workloads 
   jobs    
   tasks  

We need computer systems to carryout tasks:
===========================================
Computer/systems:
1. Bare Metal / HardWare components 
      RAM - memory 
      Cpu 
      ROM - hard disk / volume / storage 
      MOUSE
      KEYBOARD
      Screen
2. Software components 
      operating system = OS [This is the heart of a computer] : 
        Windows OS
        MacOS 
        Solaris  
        Linux  OS:
          Radhat 
          ubuntu 
          centos 
          debain / amazon Linux / suse / etc.  
      and
      other softwares :
         shell 
         Sublime text
         mobaXterm / gitbash / telegram /    
         Microsoft word/Excell  

Examples of workloads:
  fileMGT / userMGT / packageMGT/ securityMGT / systemMGT / etc.

Workload management on Computer systems [LINUX OS] :
    GUI: = Graphical user interface  -- 5%
    CLI: = command line interface    -- 60%
            aws ec2 describe-instances  
     Linux OS = Linux servers/systems
      ls:   = list the content of a directory
      touch test.txt

scripts:
======== 
A shell-script is a collection of one or more commands in a file or it's a file containing commands 

write a simple script that welcomes Engineers to work?


welcome.sh
==========

         #!/bin/bash 
         echo "Good morning"
         whoami
         echo "Welcome to solavisetech" 
         echo "Today is"
         date 



run the script by:
-----------------

       ./scriptName

       ./welcome.sh
       ./script1.sh
  
 The file/script need executable Permissions to run  
    chmod 744 welcome.sh  
    chmod  u+x scriptName 
    chmod   +x scriptName  

Assign executable Permission:
  chmod +x fileName   
  chmod +x script1.sh
  chmod 775 fileName 
  chmod 700 fileName 

shell: A shell is an interpreter that interpretes commands to the OS. 

shells command interpreters:
  Boune Shell  (sh)
  Boune Again Shell (bash)
  csh / ksh / tsh / zsh  

  echo $SHELL       =  List your current shell
      /bin/bash
  cat /etc/shells   = List all shells in your system
     /bin/sh
     /bin/bash
     /usr/bin/sh
     /usr/bin/bash
     /bin/csh
     /bin/tcsh
     /usr/bin/csh
    /usr/bin/tcsh

sudo yum install ksh zsh -y 

/bin/sh
/bin/bash
/usr/bin/sh
/usr/bin/bash
/bin/csh
/bin/tcsh
/usr/bin/csh
/usr/bin/tcsh
/usr/bin/zsh
/bin/zsh
/bin/ksh
/bin/rksh
/usr/bin/ksh
/usr/bin/rksh

  bash -c ls  or ls   

Bash shell Scripting:
====================

Naming convention:
Naming conventions best practices:
bash Shell-scripts   = script.sh or hello.sc  
Shell-scripts has '.sc' or '.sh' extensions 
    scriptname.sh  or scriptName.sc

    *.sh 
    *.sc

  deploy.sh  = Shell-script [*.sh]
  test.txt   = text file    [*.txt]
  app.sc     = Shell-script [*.sc]
  app.java   = java code    [*.java] 
  monitor.py = python code/script [*.py] 
  app.yaml   = playbook or manifest file [*.yml] 
  main.tf    = terraform scripts/codes [*.tf]

script1.sh
---------

#!/bin/bash
echo "Good morning Millionaire,"
whoami
echo Welcome to solavisetech 
echo Today is,
date


Scripting/automation langauges:
  1. Bash shell
  2. Python 
  3. Groovy  (Jenkins)
  3. Ruby
  4. Yaml  
      (k8s, Ansible, CloudFormation)
  5. JSon / java
  6. HCL - Terraform  
  7. XML = 
  8. html 
  9. go/golang 
  10. powershell 

Tasks
=====

write a simple shell script to deploy applications 
1. Create a deployment directory  
2. create a deployment; app.java file  
3. assign read Permission to app.java file
4. Create a user moses
5. change ownership of app.java file to moses
6. Create app directory 
7. copy the file to the app directory 
      

How to make your codes/scripts:
  easily readable/understandable 
  1. by adding notes/comments/explanations 

comment.sh
----------

  #!/bin/bash
  echo 'single line comment starts'
  # This script welcome Engineers to solavisetech.
  # comented lines starts with #
  # Only run this script on Linux systems
  # Author:ATANGA
  # Copyright C solavisetech
  # whoami
  date
  echo welcome to solavisetech
  echo 'single line comment ends'

mlc.sh
------
  #!/bin/bash
  echo "Multi-line comment starts"
  <<boy
  This script welcome Engineers to solavisetech.
  Only run this script on Linux systems
  Author: Prof. Atanga
  Copyright C Solavisetech
  pwd
  boy
  echo "Multi-line comment ends"
  date
  whoami

ANOTHER
-
  <<rich
  This script welcome Engineers to solavisetech.
  Only run this script on Linux systems
  Author: Prof. Atanga
  Copyright C Solavisetech
  pwd
  rich

Who are the comments meant for?

1. It make your script/code to be understood by you and others over time. 
2. It make your script/code easily reusable in the future
3. Facilitate/ease troubleshooting and debugging
4. comments are Good for teams: Team of 14 
6. developers writing codes/scripts 
1. Scrum master 
3. DevOps Engineers 
1. DevOps Security Engineer 

Making your script portable.  
1. Hard coding 
2. soft coding   

using variables in scripting:
============================
name=Atanga
cpy=solavisetech
how to call variables in bash shell scripting:
  $variableName 
  ${variableName} 

var1.sh  
-------

  #!/bin/bash
  name=Atanga
  cpy=solavisetech
  echo "Good morning ${name}"
  echo "Good morning ${name}"
  echo Welcome to $cpy
  echo Good morning ${name}, welcome to $cpy

variables:
variables are defined by the either the user or the system 
we can refer/call a variable with $variable 

User defined variables   = UDV  : 

 Are defined/created by some admins  

udv.sh
------ 

  #!/bin/bash
  name=Atanga
  cpy=solavisetech  
  city=Alexandria
  country=USA 
  echo $name works for $cpy located in $city, $country    

system defined variables   = SDV  : 
SDV Are variables that comes with the OS  
Such variables are in uppercase

SHELL=bin/bash
echo $SHELL  = /bin/bash
env = List all system defined variables  

sdv.sh
- 
city=Alexandria
APP=TeslaApplication
user=Atanga
echo $USER works for solavisetech, $city
echo $PWD
echo $SHELL
echo "This $APP is the best version in the market"
# udv are or should be written in lowercase. Highly recomended
# sdv  are written in upper case

If you run the command = env;

SHELL=/bin/bash
HISTCONTROL=ignoredups
SYSTEMD_COLORS=false
HISTSIZE=1000
HOSTNAME=demo22
PWD=/home/oke
LOGNAME=oke
HOME=/home/oke

start writing your script with shebang [#!] /bin/sh]

system defined variables:
echo sdv starts  
echo $HISTSIZE  
echo $USER 
echo $HOME  
echo $PATH  
echo $LOGNAME
echo $SHELL 
echo sdv ends   

echo $HISTSIZE
1000
export HISTSIZE=2000


dynamic script  :
  1. echo "$name Welcome to $cpy"  

static script:
  1. echo "Atanga welcome to solavisetech"    

User defined variables:
var1.sh 
   name=Atanga 
   cpy=solavisetech
   echo "$name Welcome to $cpy"  

write a script to authenticate bank users:
==========================================

bank.sh
-------

  #!/bin/bash
  echo 'Please enter your name'
  read name
  echo "$name, welcome to TD Bank"
  echo 'please enter your card'
  echo 'please enter your pin'
  read pin
  echo "$pin is the correct pin, $name, how may we help you today?"

======================================
TICKET: Write a scipt to dynamically create users. 
   userMGT commands: adduser / usermod / userdel /  groupadd / groupdel 
      sudo adduser/userdel/usermod/ groupadd / groupdel 

userCreate.sh  
-------------

  #!/bin/bash
  # This script requires root/sudo access
  # This is a Dynamic script to create and assign passwd for users
  echo "Please enter the name of the user"
  read user
  echo "System ready to create account for $user"
  sudo adduser  $user
  echo "$user account is created successfully"
  sudo passwd $user
  sudo grep $user /etc/passwd # to verify
  sudo cat /etc/shadow | grep $user
  sudo groupadd devops
  sudo usermod -aG devops $user


IQ:
- 
Explain your experience in shell scripting  ?
1. using bash shell scripts for userMGT. 100% [New Graduate]    
2. In my environment/company/Solavisetech i have used scripting for userMGT for over 5 years. 

userMGT.sh
----------

  #!/bin/bash   
  echo "creating a newuser account" 
  echo "enter the new username's name"
  read name  
  sudo adduser $name
  sudo groupadd manager 
  sudo usermod -aG manager $name   
  id $name 

bank.sh   
-------

  #!/bin/bash
  echo "Please enter your name"
  read name
  echo "$name, welcome to TB Bank"
  echo "Please enter your pin"
  read -s pin  # -s pass a secret variable
  echo "$name you entered an invalid pin"


======================================================================================================================================================================



Inequality signs :
=================
-eq  or  == represent equals to 
           (( $? == 0 )) [ X -eq = y]
-ne  or  != represent not equals to 
-gt  or  >  represent greater than
-lt  or  <  represent less than 
-ge  or >= greater than or equals to
-le  0r <= less than  or equals to 


if else conditions
==================

if [ votes -gt 50% ]
then 
echo he won the elections 
fi  

conditions :
if statement  
Syntax:
if (( conditions ))
then 
commands 
else  
commands  
fi

if1.sh  
------

#!/bin/bash
echo "welcome to solavisetech" 
echo "How much are you willing to pay"
read price
if [ $price -ge 4000 ]
then 
echo "your are admitted"  
else  
echo "sorry you can't be admitted today "
fi  

if2.sh
------

#!/bin/bash
echo "Please enter for pin"
read -s pin  
if (( $pin == 4100 ))
then 
echo "You have entered the correct pin"
echo "Thank you for banking with TD Bank"
else  
echo "sorry you entered the wrong pin"
echo "your account is blocked for your protection"
echo "Please visit a branch for further assistance"
fi  


IQ:
-
How do you troubleshoot issues in scripting??
run the script in debugging mode  
sh -x scriptName   

Debugging problems in scripting  
===============================
  
  sh -x scriptName

Team:
-
project 1
========
1. AWS Accounts are created for all team members 
2. Create a redhat8 linux server 
3. Connect to the redhat8 server using mobaXterm/terminal ssh-cleint 
4. Program or configure the server for password authentication   
5. Create a user call dominion and assign a password [admin123] 
6. Connect to your server using dominion's user
7. Run commands in the server as dominion's user
