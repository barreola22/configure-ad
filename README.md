<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>On-premises Active Directory Deployed in the Cloud (Azure)</h1>
This tutorial outlines the implementation of on-premises Active Directory within Azure Virtual Machines.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How to Deploy on-premises Active Directory within Azure Compute](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>High-Level Deployment and Configuration Steps</h2>

- Step 1
- Step 2
- Step 3
- Step 4
- Step 5
- Step 6

<h2>Deployment and Configuration Steps</h2>

Implementing on-premises Active Directory within Azure Virtual Machines involves the following steps:

1. Set up a Virtual Network: The first step is to create a virtual network in Azure. This network will provide connectivity between the on-premises Active Directory and Azure Virtual Machines. Ensure that the virtual network has a subnet that can be used to deploy virtual machines.

2. Set up a Domain Controller: Next, deploy a virtual machine within the Azure Virtual Network and install the Active Directory Domain Services role. Configure the server as a domain controller for the on-premises Active Directory. Ensure that the server has a static IP address and is configured with DNS and DHCP services.

3. Join Azure Virtual Machines to the Domain: Once the domain controller is set up, deploy additional virtual machines within the virtual network and join them to the on-premises Active Directory domain. Ensure that the virtual machines are configured with the correct DNS settings, and that they can communicate with the domain controller.

4. Set up Site-to-Site VPN: To enable communication between the on-premises Active Directory and Azure Virtual Machines, set up a Site-to-Site VPN connection between the Azure Virtual Network and the on-premises network. This can be done using Azure VPN Gateway and a VPN device located in the on-premises network.

5. Configure Active Directory Replication: To ensure that the on-premises Active Directory and the Azure Virtual Machines are in sync, configure Active Directory replication between the domain controller in Azure and the domain controllers in the on-premises network.

6. Enable Azure Active Directory Domain Services: If you need to provide Azure Active Directory services to your Azure Virtual Machines, enable Azure Active Directory Domain Services within the Azure Virtual Network. This will allow you to join Azure Virtual Machines to an Azure-managed domain, and provide services such as LDAP, Kerberos, and NTLM authentication.
