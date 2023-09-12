# azure-network-protocols
<p align="center">
<img src="https://i.imgur.com/Ua7udoS.png" alt="Traffic Examination"/>
</p>

<h1>Network Security Groups (NSGs) and Inspecting Traffic Between Azure Virtual Machines</h1>
In this tutorial, we observe various network traffic to and from Azure Virtual Machines with Wireshark as well as experiment with Network Security Groups. <br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Various Command-Line Tools
- Various Network Protocols (SSH, RDH, DNS, HTTP/S, ICMP)
- Wireshark (Protocol Analyzer)

<h2>Operating Systems Used </h2>

- Windows 10 (21H2)
- Ubuntu Server 20.04

<h2>High-Level Steps</h2>

- Create resources
- Observe ICMP Traffic
- Observe SSH Traffic
- Observe DHCP Traffic
- Observe DNS Traffic
- Observe RDP Traffic

<h2>Actions and Observations</h2>

<p>
<img src="https://i.imgur.com/PiZmWhU.png" height="40%" width="40%" alt="Windows VM"/>
<img src="https://i.imgur.com/kspHyex.png" height="40%" width="40%" alt="Linux VM"/>
<br />
<img src="https://i.imgur.com/0awI1yS.png" height="20%" width="20%" alt="Vnet"/>
</p>
<p>
Create a Resource Group.
<br />
Create a Windows 10 Virtual Machine (VM).
<br />
While creating the VM, select the previously created Resource Group.
<br />
While creating the VM, allow it to create a new Virtual Network (Vnet) and Subnet.
<br />
Create a Linux (Ubuntu) VM.
<br />
While create the VM, select the previously created Resource Group and Vnet.
<br />
Observe Your Virtual Network within Network Watcher.
</p>
<br />

<p>
<img src="https://i.imgur.com/irUGL73.png" height="20%" width="20%" alt="Wireshark"/>
<img src="https://i.imgur.com/cZ3frp9.png" height="15%" width="15%" alt="ICMP"/>
<br />
<img src="https://i.imgur.com/8HR8n21.png" height="60%" width="35%" alt="First Ping"/>
<img src="https://i.imgur.com/7zeUNDI.png" height="40%" width="40%" alt="Ping Google"/>
<br />
<img src="https://i.imgur.com/CkwGshP.png" height="40%" width="40%" alt="Ping -t"/>
<br />
<img src="https://i.imgur.com/Lly14GL.png" height="15%" width="15%" alt="Deny ICMP"/>
<br />
<img src="https://i.imgur.com/TYwOpMk.png" height="25%" width="25%" alt="Request Timed Out"/>
</p>
<p>
Use Remote Desktop to connect to your Windows 10 Virtual Machine.
<br />
Within your Windows 10 Virtual Machine, Install Wireshark.
<br />
Open Wireshark and filter for ICMP traffic only.
<br />
Retrieve the private IP address of the Ubuntu VM and attempt to ping it from within the Windows 10 VM.
<br />
Observe ping requests and replies within WireShark.
<br />
From The Windows 10 VM, open command line or PowerShell and attempt to ping a public website (such as www.google.com) and observe the traffic in WireShark.
<br />
Initiate a perpetual/non-stop ping from your Windows 10 VM to your Ubuntu VM.
<br />
Open the Network Security Group your Ubuntu VM is using and disable incoming (inbound) ICMP traffic.
<br />
Back in the Windows 10 VM, observe the ICMP traffic in WireShark and the command line Ping activity.
<br />
Re-enable ICMP traffic for the Network Security Group your Ubuntu VM is using.
<br />
Back in the Windows 10 VM, observe the ICMP traffic in WireShark and the command line Ping activity (should start working).
<br />
Stop the ping activity
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
