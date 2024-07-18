<p align="center">
<img src="https://i.imgur.com/Ua7udoS.png" alt="Traffic Examination"/>
</p>

<h1>Inspecting Traffic Between Azure Virtual Machines</h1>
In this lab, I observe different kinds of network traffic to and from Azure virtual machines with Wireshark as well as experiment with network security groups. <br />



<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop Connection
- Command-Line Tools
- Various Network Protocols (SSH, RDH, DNS, HTTP/S, ICMP)
- Wireshark (Protocol Analyzer)

<h2>Operating Systems Used </h2>

- Windows 10 Pro (22H2)
- Ubuntu Server 20.04

<h2>VM Configuration</h2>

Within Azure, I created two VMs within the same virtual network to ensure that they are able to communicate with each other. One VM will have Windows 10 Pro while the other uses Ubuntu. The Windows VM will connect to the other via the command line/PowerShell. 

<h2>Actions and Observations</h2>

<p align="center">
<img src="https://github.com/user-attachments/assets/8c4330fa-1f1f-4521-a919-67119ce787ea" height="70%" width="70%" alt="Azure Networking Steps"/>
</p>

- Using Remote Desktop Connection, I connected to the Windows VM and installed Wireshark to begin inspecting network traffic.
<br />

<p align="center">
<img src="https://github.com/user-attachments/assets/56a9bf6c-32e6-4a56-bdbe-b49da6604f2e" height="70%" width="70%" alt="Azure Networking Steps"/>
</p>

- With Wireshark running, I filtered ICMP (Internet Control Message protocol) traffic and used PowerShell to execute a ping command. The ping command utilizes ICMP, and it can be used to test for communication between two devices. In this case I will test if my Windows VM and communicate with the Linux VM using its private IP Address. I was able to successfully inspect every reply/request between the two VMs. To inspect network traffic from a server outside of our local Virtual Network, I tested the ping command on google.com and also successfully recieved reply/request packets.
</br>
 
<p align="center">
<img src="" height="70%" width="70%" alt="Azure Networking Steps"/>
</p>
- IN PROGRESS
</br>
