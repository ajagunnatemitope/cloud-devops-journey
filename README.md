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

The application decides it needs to save a file. It does not talk to the hardware directly — it calls a system library, a pre-built tool the OS provides. The system library passes the request to the operating system, which checks whether the application has permission to write files. The OS passes the instruction to the kernel, which handles the actual technical communication with the hardware. The hardware — specifically the storage drive — physically writes the data.

The Shared Responsibility Model — OS Layer

Who is responsible for the OS on a cloud server — 
The customer is responsible the operating system on the cloud server. AWS is only responsible for the hardware components. Example is the situation with a landlord and tenant. The landlord is responsible for the building, the tdenant is responsible for its property within that building. If the tenant leaves his or her door open and get robbed the landlord will not be responsible for the theft. Also the type of furniture used by the tenant is not a concern with the landlord.


Real Scenario — OS Mismatch

Describe what happens when an application built on Ubuntu is deployed on Amazon Linux, why it fails, and how you would fix it.

An application built on ubuntu might fails on amazon linux due to different distros used. To fix it, first is to confirm what the application is really build on either ubuntu or amazon linux and if it supports it. Afterwards, either configure it to work with amazon linux or change the code



Why This Makes Me a Better Engineer

Learnt alot and most of my why question are getting abnswered with the lessons.

[x] Module 1 — How Computers Actually Work
[x] Module 2 — Operating Systems



