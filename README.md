# post-install-config
<p align="center">
<img src="https://i.imgur.com/tUnlhRz.jpeg" height="80%" width="80%" alt="Setting Up in Azure"/>
<br />

<h1>osTicket: Post-Installation Configuration</h1>


<h2>Description</h2>
This project focuses on configuring osTicket, so it can be used properly as a ticketing system. It consists of setting up multiple agents along with their departments, roles, and permissions. As well as, configuring SLAs (Service Level Agreements), help topics, and users.<br/>
<br/>

This project is a continuation of the  [osTicket: Prerequisites and Installation](https://github.com/AH1791/osticket-prereqs) project.
<br />


<h2>Environments and Utilities Used</h2>

- <b>Microsoft Azure</b>
- <b>Virtual Machines</b>
- <b>Remote Desktop Connection</b>
- <b>osTicket</b>


<h2>Operating Systems Used </h2>

- <b>Windows 10</b>

<h2>Project Walk-through:</h2>

<p align="center">
With osTicket open navigate to the Admin Panel by clicking "Admin Panel" located in orange at the top right of the page: <br/>
 
![image](https://github.com/user-attachments/assets/94a88cc5-0377-47fa-9efe-be76adf24b2a)

<br />
<br />
To start configuring Roles Navigate to the "Agents" tab and click on "Roles" underneath the "Agents" tab. Enter a role name:  <br/>

![image](https://github.com/user-attachments/assets/acb5c5e1-53fe-44ee-885f-ab6b1a4665e6)

<br />
<br />
In the "Permissions" tab of this role, give this role all permissions in "Tickets", "Tasks", and "Knowledgebase". This will be our "Supreme Admin" Role:  <br/>

![image](https://github.com/user-attachments/assets/99a4a5a1-9c34-4427-9f08-9c307df9f1f2)

<br />
<br />
To set up departments, while still in the "Agents" tab, click on "Departments" located just below the "Agents" tab. Name the department "SysAdmins" and create the Department:  <br/>

![image](https://github.com/user-attachments/assets/2c9b16c5-dca4-432b-9294-0664d3f742fd)

<br />
<br />
Next, create a team by selecting the "Teams" tab, while still in the "Agents" tab. Then, name the team "Online Banking" and create team:  <br/>

 ![image](https://github.com/user-attachments/assets/d8756c17-fbd1-4d7d-a704-5299147d9944)

<br />
<br />
Now, to allow anyone to create tickets, go to the "Settings" Tab, and under "Authentication Settings" make sure that "Require registration and login to create tickets" is unchecked:  <br/>

![image](https://github.com/user-attachments/assets/bc36de72-6e98-4f98-a5a4-5818c84d55e3)

<br />
<br />
To create agents (the help desk workers) navigate back to the "Agents" tab and select "Agents" and fill out the name, email, and username:  <br/>

![image](https://github.com/user-attachments/assets/424c3c20-eb73-4b25-8b30-584d4fd1de9e)


<br />
<br />
Next to the username click "Set Password" set the password. Uncheck the "Send the agent a password reset email" and "Require password change at next login" options:  <br/>

![image](https://github.com/user-attachments/assets/9bb89cf3-ceb1-4c99-82b9-0472a2fe016f)

<br />
<br />
On the "Access" tab for this user select the "SysAdmins" department and the "Supreme Admin" role created earlier:  <br/>

![image](https://github.com/user-attachments/assets/e559a9fc-1c8e-4b18-b450-5cd85f9ba57b)

<br />
<br />
Under the "Teams" tab select "Online Banking" for this agent:  <br/>

 ![image](https://github.com/user-attachments/assets/f5d7bd7e-5bd6-4270-a567-139a84e25ef6)

<br />
<br />
Create one more agent as done previously, the only difference is in the "Access" tab select "Support" for the department:  <br/>

![image](https://github.com/user-attachments/assets/dc0f2e52-8f69-49e1-9b84-e50fcec4f3eb)
![image](https://github.com/user-attachments/assets/9943f09f-78b4-4082-9ebc-ff37f3839528)


<br />
<br />
<img 
<br />
<br />
Next, to create a user (the customers) switch to the "Agent Panel" in orange in the top right> Users> Add User and put an email and name, then create. (I also made one more user with the same steps taken here):  <br/>
<img 
<br />
<br />
Configuring an SLA plan navigate back to Admin Panel> Manage> SLA create three SLAs with different severities, grace periods, and schedules like so:  <br/>
<img 
<br />
<br />
<img 
<br />
<br />
<img 
<br />
<br />
Under the same "Manage" tab go to the "Help Topics" tab and create four help topics named, "Business Critical Outage", "Personal Computer Issues", "Equipment Request", and "Password Reset" all with the same settings like so:  <br/>
<img 
<br />
<br />


<h2>osTicket Setup Complete!</h2>

<b> We've successfully set up multiple agents along with their departments, roles, and permissions. As well as, configured SLAs (Service Level Agreements), help topics, and users! osTicket is now setup for the next project where I will create and work different tickets using multiple agents and users!  </b>
<br />
<br />
</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
