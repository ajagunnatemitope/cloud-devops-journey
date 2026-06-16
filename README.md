About This Repository

This repository documents my learning journey from zero experience to Cloud DevOps Engineer. Each module adds new concepts, labs, and projects.

Module 1 — How Computers Actually Work

The Four Components of Every Computer

CPU:
Central processing Unit. Its the brain behind the computer, every processes is done by it. When it is overwhelmed it slows down the application

RAM:
Random access memory is the temporary storage of the computer, it stores any processes temporarily being processes by the CPU. It does not store any information hence when the compouter off it does not survive it unlike thge storage which is not affected by power.

Storage:
This is where all the information and other relevant activities to be stored are done for a long time. It can be in disk or ssd

Network Interface:
This is the interface that allows communication between an application or server. It sends and receive data from other computers

What is Virtualisation? This is the use of hardware components virtually without the physical components being present

What is a Hypervisor? Hpervisor is a softwrae that sits on the hardware of a computer that allows the allocation of vitual machine from a cloud infrastructure

What is a Cloud Server? this is a server that is hosted in the cloud and can be accessed without having the physical hardware in the same location

The shared responsibility Model entails all hardware components are to be responsible to by AWS. Password and how the environment is set up depends on the cloud server owner
aws is not responsible for leaked password compromise account. For example, if a company gets hacked because of a weak password, that is the company's responsibility, not AWS's. But if a physical server in Amazon's data centre fails, that is Amazon's responsibility. If a physical server catches fire, Amazon replaces it. If there's a power cut to the data centre, Amazon's backup generators kick in. If the hypervisor has a bug, Amazon patches it.

AWS is responsible for the hardware and setup of the clous infrastructure. If anything goes wrong with the hardware, AWS is responsible for it. The client is only responsible for their own allocated slot given by AWS, their security measures.

The concepts of how computer works gives me a background of the origin and what it does accordingly.

## Module 2 — Operating Systems


What Is an Operating System? The operating system is a software, rather it is in charge of managaing all processes in the computer, The operating system determines what is allocated to the processes of an application and how it process its data.

The Kernel - The kernel is the one which manages memory allocation

Why Linux Dominates Cloud Infrastructure

Linux dominates cloud intrastructure because it is free, developers prefers it than spending thousands on a windows operating system, it is opensource, it is lighweight and can be left without a restart for a long time

The OS Stack

The application decides it needs to save a file. It does not talk to the hardware directly — it calls a system library, a pre-built tool the OS provides. The system library passes the request to the operating system, which checks whether the application has permission to write files. The OS passes the instruction to the kernel, which handles the actual technical communication with the hardware. Kernel manages memory allocation, it controls which processes get CPU time, it is the reason some operations require special permissions. The hardware — specifically the storage drive — physically writes the data.

The Shared Responsibility Model — OS Layer

Who is responsible for the OS on a cloud server — 
The customer is responsible the operating system on the cloud server. AWS is only responsible for the hardware components. Example is the situation with a landlord and tenant. The landlord is responsible for the building, the tdenant is responsible for its property within that building. If the tenant leaves his or her door open and get robbed the landlord will not be responsible for the theft. Also the type of furniture used by the tenant is not a concern with the landlord.


Real Scenario — OS Mismatch

Describe what happens when an application built on Ubuntu is deployed on Amazon Linux, why it fails, and how you would fix it.

An application built on ubuntu might fails on amazon linux due to different distros used. To fix it, first is to confirm what the application is really build on either ubuntu or amazon linux and if it supports it. Afterwards, either configure it to work with amazon linux or change the code



Why This Makes Me a Better Engineer

Learnt alot and most of my why question are getting abnswered with the lessons. I know more about operating systems which strenghthens my judgement about CPU, storage, kernel in troubleshooting. When an application is slow now, i know how to navigate in my troubleshooting steps by answering the right questions. 


[x] Module 1 — How Computers Actually Work
[x] Module 2 — Operating Systems

Module 3 — The Command Line
What Is the Command Line? Command line is a terminal used to pass instructions or communicate with application servers

The command line exist because it is fast, efficient and manual. Engineers prefer it over graphical user interface becasue not only does it diagnose, issues can also be resolved there also. It also hasndles automation. 

An engineer can run diagnostics, detect issues automatically, solve issues and also automate commands.

The Commands I Now Know

For each command below write one sentence explaining 
what it does and when you would use it on the job:
pwd - print working directory it is to know exactly where i am and what i am working on. ls -la - this is to list the files in the directory and it also shows hidden files, cd - change directory, this is to change from one working directory to the other. cat - this is used to read a file. touch - touch is used to create a file. mkdir -p -  this is used to create a durectory and its sub folders, cp - this is used to copy a file and it is always necessary to use it when commiting a major change, always duplicate the file before proceeding, mv - this is used to move a file or rename a folder, rm -rf - this is used to delete, it is iorreversable and should be used with care, tail -f - this is used to read log in real time as they are written, often used to see the error as they appear or occur, grep - this is used to fetch a particular pattern in a log file e.g ERROR, FATAL, history - this is used to check the history of all command that has been entered on the terminal, whoami - this is used to checked the user currently working on, engineers often log in as different users, this enable you know the exact user you are logged as, chmod - change mode, this is used to grant permission, chown - change owner, it is used to change the owner or permissions of a file or folder, sudo - this is the root user, it overrides permissions.

Permissions and Least Privilege

Permission string system isa system that ensures permission or task is only granted to an emp0loyee with the specific task assisgned to do. It is necessary as if every employee has all permissions and an employee is compromised it can allow the enter system to be compromise through the user. 

The Pipe

The pipe is a connector that takes the result of an output and feeds it in the nect input. tail -f hpy.log | grep "ERROR" > error.txt

this takes real time logs and search for ERROR and save the logs in error.txt file

Real Scenario — Log Investigation

Describe the workflow you would follow if a developer told you the application was throwing errors. 
Which commands, in which order, and why.

tail -f - this shows me the logs in real time
grep - to grep the error

What I Built in This Lab

Link to your linux-lab-cloudproject repository. https://github.com/ajagunnatemitope/linux-lab-cloudproject

I have learnt different linux commands, i made a directory, move files in it and also searched for errors. I have learnt a lot of things which gives me an edge from when i first came. 
Progress Tracker

[x] Module 1 — How Computers Actually Work
[x] Module 2 — Operating Systems
[x] Module 3 — The Command Line

