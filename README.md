# DemoExam26
# Instructions for the stand

### The infrastructure setup is divided into logical phases. It is highly recommended to follow the sequence: start with Windows Server (DC1 and DC2) deployment, followed by Client1 and Ubuntu configuration.

## Node Roles:
``DC1 (Primary Domain Controller)``: The heart of the infrastructure. It serves as the foundation for Active Directory and acts as the Network Gateway, providing internet access to the internal network via NAT.

``DC2 (Additional Domain Controller)``: Provides high availability and fault tolerance through AD replication. It ensures the network remains operational if DC1 fails.

``Client1 (Workstation)``: A standard domain-joined user machine. In this scenario, it is used to simulate user activity and perform security testing on the DVWA application.

``Ubuntu (Vulnerable Server)``: The vulnerable segment of the network. It hosts the web server (Apache + DVWA) and, along with the domain controllers, forms the core server environment of the lab.
















  
