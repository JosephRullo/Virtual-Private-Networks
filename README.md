<p align="center">
<img src="https://i.imgur.com/Gepl8Q5.jpg" alt="Microsoft Active Directory Logo"/>
</p>

<h1> <p align="center"> Virtual Private Network Connections</h1>
<p align="center"> This tutorial outlines the implementation and connection to Virtual Private Networks and how they affect your IP address.<br />
<br />
<br />
<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Proton VPN

<h2>Operating Systems Used </h2>

- Windows 10 (21H2)
<p>
<p>
<p>
<br> 
<h2>Let's briefly describe how Virtual Private Networks work</h2> A VPN is a tool that allows you to access the internet securely wherever you are. It works by creating a secure “tunnel” between your device and your VPN provider, and it protects you in two key ways. 
<p>  
<p>  1. Concealing your IP address, protecting your identity and location 
<p>  2. Encrypting your traffic between you and your VPN provider so that no one on your local network can decipher or modify it.
<br>
<br>
For the example below I will create a Virtual Machine in Microsoft Azure and assign it a region in another country. Then I will demonstrate how a VPN can be used to change the IP address and view yet anoter regions local content as if it physcially located there. The diagram below will illustrate this.
<p>
<p>
<img src="https://i.imgur.com/NdcDaMC.png" alt="Microsoft Active Directory Logo"/> <height="60%" width="60%" alt="Disk Sanitization Steps"/> 
  
<h1>Implementation</h1>
<br>
<h2>Step 1.</h2>

**Create a Virtual Machine in Azure**
<p>
For this tutorial we will be demonstrating the VPN connection within a Virtual Machine (click here for a VM tutorial (https://github.com/JosephRullo/Azure-Virtual-Machines-and-Networking). Select a region outside of where you are located, in this example I've chosen Japan. Take note of the Public IP Address and Location on the VM overview page.
<p>
<p>
<img src="https://i.imgur.com/nVwElfM.png" alt="Microsoft Active Directory Logo"/> <height="60%" width="60%" alt="Disk Sanitization Steps"/> 
<img src="https://i.imgur.com/8y5iyce.png" alt="Microsoft Active Directory Logo"/> <height="60%" width="60%" alt="Disk Sanitization Steps"/> 
<p>
<br>
<h2>Step 2.</h2>

**Log in and Check your IP Address**
<p>
Log into the VM via Remote Desktop. Once Window's is done booting, go to the web browser and go to this website (www.whatismyipaddress.com). This will show you the actual IP Address and Region that was created for the VM. Next try going to (google.com), and notice the native language of the region is displayed. 
<p>
<p>
<img src="https://i.imgur.com/QvpRM8Q.png" alt="Microsoft Active Directory Logo"/> <height="60%" width="60%" alt="Disk Sanitization Steps"/> 
<img src="https://i.imgur.com/X19xJQN.png" alt="Microsoft Active Directory Logo"/> <height="60%" width="60%" alt="Disk Sanitization Steps"/> 
<p>
<br>
<h2>Step 2.</h2>

**Download and Install a VPN Client**
<p>
Select a VPN client that you would like to download and install, there are many options to choose from. For this example I will be using Proton VPN, which has a free version available here (https://protonvpn.com/). Once downloaded open the app and sign in. 
<p>
<p>
<img src="https://i.imgur.com/IPUb2fV.png" alt="Microsoft Active Directory Logo"/> <height="60%" width="60%" alt="Disk Sanitization Steps"/> 
<p>
<br>
