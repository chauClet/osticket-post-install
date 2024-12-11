<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configurations</h1>
This lab demonstrates the necessary changes I make to configure osTicket so it can be used as a proper ticketing system.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop Connection
- osTicket 

<h2>Operating Systems Used </h2>

- Windows 10 Pro</b> (21H2)


<h2>Configuration Steps</h2>

![Screenshot 2024-12-05 220157](https://github.com/user-attachments/assets/3a56b6b7-2c07-4127-8929-04721d83415f)

After installing osTicket, it is now time to make configurations to use it as a ticketing system. One thing to note is that I switch between Admin and Agent panels as each panel has different configurations. To tell which panel is used, look at the top right of the osTicket screen. If it reads Agent Panel, the Admin panel is the one being used and vice versa.

![Screenshot 2024-12-09 232006](https://github.com/user-attachments/assets/32db2bf7-4f3d-4a3d-aee8-3be643d39141)

The first step to take is to make a new role called Supreme Admin. For the purposes of this lab, I am intentionally creating a role that has every permission that can be granted. To create a new role, open the Admin panel enter the Agents Menu. Click on Roles and create the new role from there.

![Screenshot 2024-12-09 233208](https://github.com/user-attachments/assets/37dcb8bd-628b-4ac1-b785-6de96d5ddaf6)

Next, a new Department will be created for System Administrators. In the Admin panel, open the Agents menu and click on Departments to create a new Department within osTicket.

![Screenshot 2024-12-09 233944](https://github.com/user-attachments/assets/304df40a-1a8c-4e3c-9025-962a5652e850)

A new Level II Support Team will have to be created to supplement the Level I Support Team already made within osTicket. To create a new Team, enter the Admin panel and open the Agents menu. Click on Teams and add any new teams that need to be created.

![Screenshot 2024-12-09 234700](https://github.com/user-attachments/assets/6f1cc20a-605c-4f70-9dda-ff45511a0ac9)

New agents will have to be created so they can take tickets that come to the queue. To create new agents, enter the Admin panel and open the Agents menu. Click on Add New Agent and create the account credentials for each new agent. In this case, Jane and John Doe are created.

![Screenshot 2024-12-09 235505](https://github.com/user-attachments/assets/92fe5946-3f6a-43ee-915a-068d73e7f259)

New users will be created so they can create tickets so that the agents can receive and triage them. To create new users, enter the Agents panel and open the Users menu. Click on Add User and create the account credentials necessary for each new user. In this case, Karen and Ken have been created.

![Screenshot 2024-12-09 235602](https://github.com/user-attachments/assets/3d4e14c5-b99f-4600-a677-50a01edcc391)

Service Level Agreements (SLAs) will have to be made in order to categorize tickets according to their level of impact. To make new SLAs, enter the Admin panel and open the Manage menu. Click on SLA and create any needed SLAs. In this case, SEV-A, B, and C have been created to categorize tickets that need to be resolved within 1 hour, 4 hours, and 8 hours respectively.

![image](https://github.com/user-attachments/assets/2fb42d01-ff57-4e9f-a603-b44c003e9d69)

Finally, Help Topics need to be created to help users select an appropriate category that describes their problem so that Agents get an idea of what problem is described in the ticket. To make a new Help Topic, enter the Admin panel and open the Manage menu. Click on Help Topics and click on Add New Help Topic. In this case, I have added the following in order to use later for when I create new tickets to resolve: Business Critical Outage, Personal Computer Issues, Equipment Reset, and Password Request.

<h2>osTicket Configurations are Complete </h2>

Now that the configurations have been set in place, I can now utilize osTicket as a proper ticketing system. I can create tickets and be able to traige them as if I were in a real environment.
