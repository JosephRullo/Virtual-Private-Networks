<p align="center">
<img src="https://i.imgur.com/Gepl8Q5.jpg" height=100% width=100% alt="Microsoft Active Directory Logo"/>
</p>

<h1> <p align="center"> Virtual Private Network Connections</h1>
<p align="center"> This tutorial outlines the implementation and connection to Virtual Private Networks and it's affect on IP addresses.<br />
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
<h2>Step 3.</h2>

**Download and Install a VPN Client**
<p>
Select a VPN client that you would like to download and install, there are many options to choose from. For this example I will be using Proton VPN, which has a free version available here (https://protonvpn.com/). Once downloaded open the app and sign in. 
<p>
<p>
<img src="https://i.imgur.com/IPUb2fV.png" alt="Microsoft Active Directory Logo"/> <height="60%" width="60%" alt="Disk Sanitization Steps"/> 
<p>
<br>
<h2>Step 4.</h2>

**Select a VPN Connection**
<p>
Once signed in, you will be brought to a screen showing your current IP Address and status. This is where you can choose where you would like to establish the VPN server. For this example I will choose the Netherlands. Select the country and click connect. Once the connection is established, observe the changes on the VPN status screen.
<p>
<p>
<img src="https://i.imgur.com/yPCYU0t.png" alt="Microsoft Active Directory Logo"/> <height="60%" width="60%" alt="Disk Sanitization Steps"/> 
<img src="https://i.imgur.com/RwZW2gk.png" alt="Microsoft Active Directory Logo"/> <height="60%" width="60%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/3HGzqQH.png" alt="Microsoft Active Directory Logo"/> <height="60%" width="60%" alt="Disk Sanitization Steps"/>
<p>
<br>
<h2>Step 5.</h2>

**Verify VPN is Working**
<p>
Now that we've established a VPN connection, let's go back to the web browser an check our IP (www.whatsmyipaddress.com). Notice now that it is showing the new location we connected to. We are now browsing from this new location as if we were physically located there. Try www.google.com again. 
<p>
<p>
<img src="https://i.imgur.com/1t61U8o.png" alt="Microsoft Active Directory Logo"/> <height="60%" width="60%" alt="Disk Sanitization Steps"/> 
<img src="https://i.imgur.com/PtTM2Hb.png" alt="Microsoft Active Directory Logo"/> <height="60%" width="60%" alt="Disk Sanitization Steps"/>
<p>
<br>
<h2>Step 6.</h2>

**Switch VPN Servers**
<p>
Let's try switching VPN servers to demonstrate changing locations once more. Go back to the VPN client and dissconnect it. Choose another region, in this case the U.S. and click connect.
<p>
<p>
<img src="https://i.imgur.com/Pztfnzb.png" alt="Microsoft Active Directory Logo"/> <height="60%" width="60%" alt="Disk Sanitization Steps"/> 
<img src="https://i.imgur.com/Yrh9BzT.png" alt="Microsoft Active Directory Logo"/> <height="60%" width="60%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/JdCAroM.png" alt="Microsoft Active Directory Logo"/> <height="60%" width="60%" alt="Disk Sanitization Steps"/>
<p>
<br>
<h2>Step 7.</h2>

**Check Web IP again**
<p>
Once again go back to the web and check both websites to verify the change.
<p>
<p>
<img src="https://i.imgur.com/6vDH9er.png" alt="Microsoft Active Directory Logo"/> <height="60%" width="60%" alt="Disk Sanitization Steps"/> 
<img src="https://i.imgur.com/o1d7ik0.png" alt="Microsoft Active Directory Logo"/> <height="60%" width="60%" alt="Disk Sanitization Steps"/>
<p>
<br>

<h2> <p align="center"> This concludes the Virtual Private Network demonstration, thanks for viewing.</h2>
