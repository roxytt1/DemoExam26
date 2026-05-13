# Setting up Windows Server (DC1 and DC2) 
First, you need to change the name of the server itself. 

<img width="521" height="100" alt="image" src="https://github.com/user-attachments/assets/ab616365-5165-4bd5-83f7-c7e1485bb9cd" />


## AD DS

``Control`` -> ``Add roles and features`` -> ``Domain Services Acctive Directory`` 

<img width="658" height="292" alt="image" src="https://github.com/user-attachments/assets/18adfa08-3310-49ee-901a-48f71655f5f1" />

### Promote to domain controller 

<img width="658" height="292" alt="image" src="https://github.com/user-attachments/assets/d695f0c5-1d96-4b21-8180-357dedb115e9" />

### Add new forest 

<img width="658" height="292" alt="image" src="https://github.com/user-attachments/assets/bd7164e2-8a35-4be3-a37e-2999650d114b" />

## DHCP

``Control`` -> ``Add roles and features`` -> ``DHCP-server``

<img width="658" height="292" alt="image" src="https://github.com/user-attachments/assets/b1d26c58-beaf-47ea-bde5-27c76c6bf87a" />

### Complete settings DHCP

<img width="327" height="257" alt="image" src="https://github.com/user-attachments/assets/12129ce5-c8cd-40ef-b820-2be18fe9a1a9" />

### Fix

<img width="658" height="292" alt="image" src="https://github.com/user-attachments/assets/926c7bb4-5ff6-450f-aa80-7dbc8a92148f" />


``Tools`` -> ``DHCP``

<img width="569" height="137" alt="image" src="https://github.com/user-attachments/assets/c40a535c-1754-4d7e-99d1-6b736f25b06e" />


``dc1.kit.local(I just didn't change the name)`` -> ``IPv4`` -> ``New sсope``

<img width="577" height="292" alt="image" src="https://github.com/user-attachments/assets/020e4012-79b1-45ae-a986-599d6daf9142" />

#### Here we must set the starting and ending IP address in the network, all these addresses will subsequently be received by our clients and servers.

``Initial IP address - 192.168.10.1``

``Final IP address - 192.168.10.100``

<img width="514" height="292" alt="image" src="https://github.com/user-attachments/assets/a5554f5d-c34a-4604-8f54-91a71737e185" />

#### Next, we add the exception addresses that will go to ``DC1`` and  ``DC2`` .

<img width="346" height="103" alt="image" src="https://github.com/user-attachments/assets/c146eeaf-cad8-4723-b044-1bb691810300" />

### Routing 

<img width="451" height="183" alt="image" src="https://github.com/user-attachments/assets/bf704aa1-8ab8-4c07-8088-20896bfc2a94" />

## NAT 

``Control`` -> ``Add roles and features`` -> ``Remote Access``
#### The main thing in Role Services is to check the "Routing" box.

<img width="658" height="292" alt="image" src="https://github.com/user-attachments/assets/dfe08d81-4e4c-406d-b969-90b178e2fb83" />

## NAT setup

``Tools`` -> ``Routing and Remote Access``

<img width="510" height="166" alt="image" src="https://github.com/user-attachments/assets/09161aaf-d07e-4a58-b1be-9d7d7ac17125" />

# End of DC1 setup
