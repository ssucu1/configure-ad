<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>Active Directory Deployed in the Cloud (Azure)</h1>
This tutorial outlines the implementation of Active Directory within Azure Virtual Machines.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>High-Level Deployment and Configuration Steps</h2>

- Step 1: Preparing AD Infrastructure in Azure
- Step 2: Deploying Active Directory
- Step 3: Creating Users with PowerShell
- Step 4: Group Policy and Managing Accounts

<h2>Deployment and Configuration Steps</h2>


![AD](https://github.com/user-attachments/assets/72d4ff31-4440-4d89-87a4-0813160edf05)

<p>
Preparing the Active Directory Infastructure in Azure.
</p>
<br />

![Screenshot (16)](https://github.com/user-attachments/assets/81db7308-b6df-4f8f-a79e-ccab0cb9a7a8)

<p>
Install Active Directory
—
Login to DC-1 and install Active Directory Domain Services
Promote as a DC: Setup a new forest as mydomain.com (can be anything, just remember what it is)
Restart and then log back into DC-1 as user: mydomain.com\labuser
</p>
<br />

![Screenshot (17)](https://github.com/user-attachments/assets/7544771f-8cc1-4e5f-8575-f88e24d9fee0)
![Screenshot (18)](https://github.com/user-attachments/assets/aa91ae8c-5c85-4179-af1d-5df5747a1200)


<p>
Create a bunch of additional users and attempt to log into client-1 with one of the users
—
Login to DC-1 as jane_admin
Open PowerShell_ise as an administrator
Create a new File and paste the contents of the script into it
Run the script and observe the accounts being created
When finished, open ADUC and observe the accounts in the appropriate OU　(_EMPLOYEES)
attempt to log into Client-1 with one of the accounts (take note of the password in the script)

</p>
<br />
