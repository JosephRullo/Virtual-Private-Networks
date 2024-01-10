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

<img src="https://i.imgur.com/Gepl8Q5.jpg" alt="Microsoft Active Directory Logo"/>
  
<h1>Implementation</h1>
<br>
<h2>Step 1.</h2>

**Create a Virtual Machine in Azure**
<p>
For this tutorial we will be demonstrating the VPN connection within a Virtual Machine. Once fi

