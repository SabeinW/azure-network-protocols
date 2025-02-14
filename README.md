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

- Create our Virtual Machines
- Ensure both VMs are in the same Virtual Network / Subnet
- Install Wireshark (Observe ICMP Traffic)
- Retrieve the private IP address of the Ubuntu VM (linux-vm) and attempt to ping it from within the Windows 10 VM
- Configure a Firewall [Network Security Group]
- observe the ICMP traffic in WireShark
- Observe SSH Traffic
- in Wireshark, start a packet capture up
- Filter for SSH traffic only From your Windows 10 VM, “SSH into” your Ubuntu Virtual Machine (via its private IP address)
- Observe DHCP Traffic
- Observe DNS Traffic
- Observe RDP Traffic






 



<h2>Actions and Observations</h2>

<p>
<img src="https://i.imgur.com/Zmq2wv0.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/SeaL7aK.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Setting up Ubuntu-24 & Windows-10 VMs with Network Security Groups (NSGs) is critical for managing network security in Azure. By inspecting traffic (ping, SSH, RDP), we confirm that network rules are correctly configured, ensuring that only authorized communication is allowed between VMs.
</p>
<br />

<p>
<img src="https://i.imgur.com/KXUgsIM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/wbU2lg8.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/gZRDCkq.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Using Wireshark to inspect ICMP traffic allows IT professionals to diagnose network problems, monitor device communications, and ensure secure and efficient traffic flow. (Wireshark is a network protocol analyzer that captures and inspects network traffic in real-time. It helps IT professionals troubleshoot network issues, analyze security threats, and monitor communications between devices.)
</p>
<br />

<p>
<img src="https://i.imgur.com/olqbPx2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/1clPkjE.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Observing ICMP traffic in Wireshark helps IT professionals diagnose network issues, enhance security, and optimize performance.
</p>
<br />

<p>
<img src="https://i.imgur.com/sOk04kJ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Configuring a Network Security Group (NSG) in Azure is crucial for network security, traffic management, and compliance. By defining inbound and outbound rules, you can restrict access to your Azure resources, block malicious traffic, and ensure only legitimate users can interact with your systems. Properly configured NSGs play a key role in safeguarding your Azure infrastructure and maintaining a secure network environment.
</p>
<br />

<p>
<img src="https://i.imgur.com/9mCEjss.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Observing SSH traffic in Wireshark is crucial for maintaining secure network practices. It helps in monitoring the health of SSH sessions, preventing unauthorized access, and detecting potential security threats. 
</p>
<br />

<p>
<img src="https://i.imgur.com/lPsblbf.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Observing DHCP traffic in Wireshark is essential for network troubleshooting, security analysis, and optimizing IP address management. By capturing and analyzing DHCP traffic, you can detect configuration issues, ensure network stability, and protect the network from malicious activity
</p>
<br />

<p>
<img src="https://i.imgur.com/LKU0viT.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Observing DNS traffic in Wireshark is crucial for network diagnostics, security analysis, and performance monitoring. It allows you to identify DNS-related issues, detect malicious activities, and optimize network performance by ensuring accurate and timely domain resolution. 
</p>
<br />

<p>
<img src="https://i.imgur.com/5B31eL8.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Observing RDP traffic in Wireshark is essential for ensuring secure remote access, troubleshooting connection issues, and detecting potential security threats like brute-force attacks, unauthorized access, and man-in-the-middle attacks. Monitoring RDP traffic also helps in maintaining network performance and enforcing security policies, ensuring that remote access remains safe, secure, and efficient.
</p>
<br />
