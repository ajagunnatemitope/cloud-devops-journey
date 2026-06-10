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


