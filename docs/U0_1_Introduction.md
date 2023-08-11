---
title:  "Introduction"
---

# Introduction

In this unit we will focus on creating the environment we will use in future units to install the Oracle database server and clients, and perform all the tasks we will learn. We could use a real server, should we have one. But that is not likely the case, so it is better and less expensive to work with virtual machines.

Among all the possible options you can choose between the following:

- VMs in VirtualBox
- VM in Microsoft Azure Cloud
- VM in Amazon Web Services

If you decide to use VirtualBox, I will provide you the .ova files to create the virtual machines in your computer. If you decide to use Ms Azure or AWS, I will show you how to create the VM in the cloud. Each solution has advantages and disadvantages. The following table shows you some of them to help you take the decision:

| Item                              | VirtualBox | Cloud                                              |
| --------------------------------- | ---------- | -------------------------------------------------- |
| PC Hard disk usage                | High       | Very low                                           |
| PC CPU requirement                | High       | Very low                                           |
| Network usage                     | Low        | High                                               |
| Use from different PC's           | Difficult  | Very easy                                          |
| Number of simultaneous running VM | Low        | Unlimited                                          |
| Velocity to create a VM           | Low        | Very High                                          |
| Usage charges                     | No         | Yes when Azure for students credit (100$) finished |
| Platform complexity | Low | High |
| Know how to use it to get a job | Medium | Very high |

As a conclusion I would say that if you don't have a very powerful PC, the cloud would be your choice. In other cases, just decide considering which characteristics are more important to you: disk usage, mobility, learning new systems...

In any case you are going to need a Windows Server to install the Oracle 11g DBMS. In a real environment the DMBS is installed in a machine inside a data center or in the cloud. The DBMS administrators rarely connect directly to this server, but they access the DBMS remotely. Thus, we will learn to connect to the DMBS from a different PC. 

Depending on your PC operating system and the availability of the client programs for it, you can decide to install the client programs in your own PC or create a client VM to install these programs. Therefore we will need:

- Windows Server 2008 or higher
- Windows 7 or higher as client (optional)

## VM's in VirtualBox

At this point you might know quite well how to work with VirtualBox. If you decide to use this system, you have to create these virtual machines:

- Windows Server 2008
- Windows 7 (optional as client)

You can find the .ova files [here](https://gvaedu-my.sharepoint.com/:f:/g/personal/j_munozjimeno_edu_gva_es/Ep5R9IIvqjpGiz0FmLGjPWkBRnE9Kb8PAeiOVoqrlTzd1A){:target="_blank"}.

Create both machines, configure them with "bridged network" and create a shared folder with your host machine to easily change files between them.

## VM's in Ms Azure

If you decide to use Ms Azure, we can use newer versions of the operating systems, as they are available in the platform. In this case we will use:

- Windows Server 2012
- Windows 10 (optional as client)

In the following section you have all the information you need to install the Windows Server:

To install the Windows 10 client, just follow the same steps that for the Server but select the following options:

- Resource group: DBMS (the one previously created)
- VM name: dbms-win10client
- Image: Windows 10 Pro, version 21H2 - x64 Gen2
- Size: Standard_DS1_v2 - 1 vcpu, 3,5
- Virtual network/subnet: 
dbms-winserver2012-oracle-vnet/default (the one previously created)

## VM's in AWS (Amazon Web Services)

In this case we will use a Learning Lab in AWS Academy. You should have an AWS Academy student account.

In the following section you have how to create the VM in AWS academy for the server.

In AWS we can only create servers but not desktop machines. Therefore, we cannot create a Ms Windows 10 or 11 desktop VM to act as a client. We can either create another Windows Server to act as client or use the client tools in our own computer.