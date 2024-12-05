# NoOfWaysToConnectFromWindowsToLinuxMachine

Method-1 : 

Steps: 1
-------------------------------------
Create EC2 machine on AWS Free tier.
-------------------------------------
Name : My-web Server[give name here]

Selected AWS Linux by default

Instance Type : t2-micro(free tier)

Create Key pair [ pem file or ppk(putty) file ]

Click Launch instance

NOTE :: For WIN-SCP & PUTTY we need to use PPK file and GIT BASH & Mobaxtram we need to use PEM file


================================================================================================
01]Using Git Bash (Command-Line SSH)
================================================================================================
Install Git for Windows : Download from https://git-scm.com.
Open Git Bash: Type the following command to SSH into the Linux machine:

chmod 400 "labpractice.pem"
ssh -i "labpractice.pem" ec2-user@ec2-52-66-251-87.ap-south-1.compute.amazonaws.com
================================================================================================


================================================================================================
02] Using MobaXterm
================================================================================================
installation MobaXterm.
----------------------
Visit the website: https://mobaxterm.mobatek.net.
Click on the Download button.
Choose between the Home Edition (free) or the Professional Edition.
Once downloaded, run the installer to set up MobaXterm on your Windows machine.


Steps:
Connect to EC2:

Open MobaXterm → Session → SSH.

Remote Host: <Public_IP_or_DNS>.[copy from ec2 machine]

Username: ec2-user.[by-default]

Click on Advanced SSH settings

click on Use private key and upload pem file or select pem file.

Click on Ok,
================================================================================================
03]. Using WinSCP (File Transfer)
================================================================================================
Steps:
Visit the website: https://winscp.net.

double click on WinSCP.  ->  Click on run   ->   Click on Accept  ->  Next  -> install  -> finish  -> close


Search WinSCP  --> Click on Launch WinSCP:  -> Click on newsite

Protocol: SFTP.
Hostname: <Public_IP_or_DNS>.  *****
Username: ec2-user.            *****
Advanced(click)
Athentication
upload private key file as(ppk file)
click on ok.
click on Login.

login as: ec2-user
It will be connected and click on terminal which is having > symbol(shift +cntrl+ t)



================================================================================================
03]. 1. Using PuTTY (SSH) (File Transfer)
================================================================================================
double click on putty
Run
Public ip(ec2 public ip)
Click on SSH --> Auth  -> Credentials
Upload private key for authentication

login as: ec2-user






