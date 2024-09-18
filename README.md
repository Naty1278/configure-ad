<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>On-premises Active Directory Deployed in the Cloud (Azure)</h1>
This tutorial outlines the implementation of on-premises Active Directory within Azure Virtual Machines.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>High-Level Deployment and Configuration Steps</h2>

- Setup resources in Azure use PowerShell to check connectivity
- Install Active Directory
- Create an Admin and Normal User Account in Active Directory
- Join Client-1 to my domain


<h2>Deployment and Configuration Steps</h2>

<p>
<img width="1111" alt="Screen Shot 2024-09-16 at 8 21 26 PM" src="https://github.com/user-attachments/assets/39e1e3b1-ca89-47dd-930e-d9f697c1e7dc">

<p><img width="858" alt="Screen Shot 2024-09-17 at 7 28 58 PM" src="https://github.com/user-attachments/assets/138aedd8-1821-4e5f-900e-7d869fbf6837">

Created a resource group, then two Virtual machine's using the same virtual network. One using Windows 10 and other using Windows Server 2022. Checked connectivity by pinging DC-1's private IP address.
</p>
<br />

<p>
<img width="775" alt="Screen Shot 2024-09-17 at 7 47 19 PM" src="https://github.com/user-attachments/assets/dfc6c64f-5463-42e2-861e-b719c3d15dce">
</p>
<p>
Converted DC-1 Virtual Machine into a Domain Controller, allows user account to exist in a domain. 
</p>
<br />

<p>
<img width="445" alt="Screen Shot 2024-09-17 at 8 37 33 PM" src="https://github.com/user-attachments/assets/29f60b99-87f4-4f96-8313-9d4354ebda9f">
</p><img width="1126" alt="Screen Shot 2024-09-17 at 8 53 05 PM" src="https://github.com/user-attachments/assets/28dfd318-9b10-43e6-b1ab-d9146e7036ff">

<p><img width="977" alt="Screen Shot 2024-09-17 at 8 57 59 PM" src="https://github.com/user-attachments/assets/4f0f091a-7ef1-413f-9b59-56dbf0080990">

Made a user an Admin by adding them to domain admins security group. Joined Client-1 onto Domain Controller and verified it in Active Directory. 
</p>
<br />
