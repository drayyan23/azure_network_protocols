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

- Create a Windows 10 Virtual Machine and Create a Linux (Ubuntu) Virtual Machine
- Observe ICMP Traffic
- Observe SSH Traffic
- Observe DHCP Traffic)
- Observe DNS Traffic
- Observe RDP Traffic

<h2>Actions and Observations</h2>

<p>
</p>
<p>
-Create a Resource Group to organize resources, then create a Windows 10 Virtual Machine (VM) within that Resource Group, allowing it to create a new Virtual Network (Vnet) and Subnet. Next, create a Linux (Ubuntu) VM within the same Resource Group and Vnet. Finally, monitor network performance by observing the Virtual Network in Network Watcher.
</p>
<br />

<p>
</p>
<p>
-Connect to Windows 10 VM via Remote Desktop, install Wireshark, filter for ICMP traffic, ping Ubuntu VM from Windows 10, monitor traffic in Wireshark. Ping a public website from Windows 10, then initiate perpetual ping to Ubuntu VM. Disable ICMP traffic in Ubuntu VM's Network Security Group, observe effects in Wireshark and ping activity. Re-enable ICMP traffic and verify resumed activity. Stop ping activity when finished.
</p>
<br />

<p>
</p>
<p>
-Filter SSH traffic in Wireshark, establish an SSH connection from Windows 10 to the Ubuntu VM, input commands, and observe SSH traffic in Wireshark. Exit the SSH connection to conclude the monitoring and analysis of SSH traffic between the two VMs, offering insights into network communication and security implications.
</p>
<br />
<p>
</p>
<p>
-Repeat these steps for the remaining serveres (DHCP, DNS, and RDP)</p>
<br />
