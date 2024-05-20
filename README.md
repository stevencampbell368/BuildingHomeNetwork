<h1>Creating a Network in Cisco Packet Tracer</h1>



 
 </h2>

<h2>Description</h2>
In this task, I created a simple network using Cisco Packet Tracer, configured the end devices, and verified connectivity.
<br />


<h2>Part 1: Building the Network</h2>
Adding the Network Devices to the Workspace To begin, I added network devices to my workspace, including a PC, a laptop, and a cable modem. The cable modem is a hardware device that enables communication with an Internet Service Provider (ISP). It connects to the ISP via a coaxial cable and to the local network via an Ethernet cable, converting the coaxial connection to an Ethernet connection.
<br />
<br />

<b>Adding the Physical Cabling Between Devices</b>
<p>1. I connected the PC to the wireless router using a copper straight-through cable, attaching it to the FastEthernet0 interface of the PC and the Ethernet 1 interface of the wireless router.</p>

<p align="center">
<img src="https://imgur.com/9IWaETb.png" height="65%" width="65%" alt="PC to the wireless router via copper straight-through cable"/>
</p>
<p>2. Next, I connected the wireless router to the cable modem with a copper straight-through cable, attaching it to the internet interface of the router and the Port 1 interface of the cable modem.</p>
<p align="center">
<img src="https://imgur.com/o1Ca7BX.png" height="65%" width="65%" alt=""/>
</p>
<p>3. Then, I connected the cable modem to the internet cloud using a coaxial cable, attaching it to the Port 0 interface of the cable modem and the Coaxial 7 interface of the internet cloud.</p>
<p align="center">
<img src="https://imgur.com/qIoAItY.png" height="65%" width="65%" alt=""/>
</p>
<p>4. Lastly, I added a laptop to the workspace, which I will connect later on.</p>
<p align="center">
<img src="https://imgur.com/ei5dySb.png" height="65%" width="65%" alt=""/>
</p>



<h2>Part 2: Configuring the End Devices and Verifying Connectivity</h2>

<b>Configuring the PC</b>
<p>1. To configure the PC for the network, I selected the Desktop tab and navigated to IP Configuration to ensure that DHCP was enabled and that the PC had received an IP address.</p>
 <p> • DHCP (Dynamic Host Configuration Protocol) assigns IP addresses to devices dynamically. In my home network, the wireless router is set up to assign IP addresses to devices that request them. If DHCP were disabled, I would have had to manually assign an IP address and configure all necessary information for the PC to communicate with other devices on the network and the internet.</p>
<p align="center">
<img src="https://imgur.com/FqA72ss.png" height="65%" width="65%" alt=""/>
</p>

<p>2. Next, I opened Command Prompt and entered the ipconfig /all command to review the IPv4 addressing information from the DHCP server. The PC received an IPv4 address of 192.168.0.2.</p>
<p align="center">
<img src="https://imgur.com/mtrxgeO.png" height="65%" width="65%" alt=""/>
</p>
<p>3. Lastly, to confirm connectivity, I used the ping command in the command prompt to ping cisco.srv. I successfully received echo reply messages.</p>
<p align="center">
<img src="https://imgur.com/BnqkRhW.png" height="65%" width="65%" alt=""/>
</p>


<b>Configuring the Laptop</b>
<p>1. To configure the laptop for wireless network access, I powered off the laptop, removed the Ethernet copper module, replaced it with the Wireless WPC300N module, and then powered the laptop back on.</p>
<p align="center">
<img src="https://imgur.com/pRok375.png" height="65%" width="65%" alt=""/>
</p>

<p>2. Next, I accessed the wireless network settings on the desktop and connected to the network.</p>
<p align="center">
<img src="https://imgur.com/7quLktP.png" height="65%" width="65%" alt=""/>
</p>

<p>3. Finally, to confirm connectivity, I opened the web browser and navigated to the cisco.srv webpage.</p>
<p align="center">
<img src="https://imgur.com/VBtzizM.png" height="65%" width="65%" alt=""/>
</p>

<p>By following these steps, I successfully created a simple network, configured the end devices, and verified their connectivity.</p>
<p align="center">
<img src="https://imgur.com/m0b9Exn.png" height="65%" width="65%" alt=""/>
</p>


<h2>Languages Used</h2>

- <b>Cisco IOS CLI (Command-Line Interface):</b> Router and Switch Configuration: Configuring interfaces, routing protocols, VLANs, and other network features. 
- <b>Bash: </b> Basic Navigation and File System Management

<h2>Environments Used </h2>

- <b>Cisco Packet Tracer - Networking Simulation Tool



<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
