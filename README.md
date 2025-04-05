<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" height="75%" width="100%"alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />


<!-- <h2>Video Demonstration</h2>

- ### [YouTube: How To Configure osTicket, post-installation](https://www.youtube.com) -->

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used</h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Configure Roles
- Configure Departments
- Configure Teams
- Configure Agents
- Configure Users
- Configure SLA
- Configure Help Topics

<h2>Configuration Steps</h2>

<h3 align="center">Configure Roles</h3>
<br />
<p>
  After logging into osTicket with Admin credentials, Go to Admin Panel > Click "Agents" > Click "Roles"
  Click "Add New Role" and name it Supreme Admin granting you it's full permissions.
</p>
<p>
  Supreme Admin:
</p>
<p>
  <img src="https://i.imgur.com/SXpTf20.png" height="75%" width="100%" alt="Definitions"/>
  <img src="https://i.imgur.com/9fBmrZj.png" height="75%" width="100%" alt="Permissions"/>
  <img src="https://i.imgur.com/1sDBsuZ.png" height="75%" width="100%" alt="More Permissions"/>
  <img src="https://i.imgur.com/2SVt7rt.png" height="75%" width="100%" alt="Even More Permissions"/>
  <img src="https://i.imgur.com/vJl5MPw.png" height="75%" width="100%" alt="Sys Admin Success"/>
</p>
<br />
<br />
<h3 align="center">Configure Departments</h3>
<br />
<p>
  Go back to Agents > Click "Departments" > click "Add New Department"
  Name it "Sysadmin" and set its parent to Top-Level.
</p>
<p>
  System Administrators:
</p>
<p>
  <img src="https://i.imgur.com/83gWQsO.png" height="75%" width="100%" alt="System Administrators"/>
  <img src="https://i.imgur.com/oGLXmQv.png" height="75%" width="100%" alt="System Administrators"/>
</p>
<br />
<br />
<h3 align="center">Configure Teams</h3>
<br />
<p>
  Go back to "Agents" again > Click "Teams" > add a new team and name it whatever you want.
</p>
<p>
  <img src="https://i.imgur.com/BnPrcDH.png" height="75%" width="100%" alt="Level II Support"/>
</p>
<br />
<br />
<h3 align="center">Allow anyone to create ticket</h3>
<br />
<p>
  Under the Admin Panel > Click on "Settings" > Go to "User Settings" > Uncheck the "Registration Required" box.
  Now unregistered users can create tickets, yhis helps in scenarios where quick ticket creation is vital.
</p>
<p>
  Make sure "Require registration and login to create tickets" is not selected:
</p>
<p>
  <img src="https://i.imgur.com/QsJjOuM.png" height="75%" width="100%" alt="ticket creations"/>
</p>
<br />
<br />
<h3 align="center">Configure Agents (workers)</h3>
<br />
<p>
  Under Admin Panel > Go to Agents > Click "Add New" 
  Here I created: Jane Doe – Department: Sysadmin, Role: Supreme Admin, Team: Online Banking. 
  And : John – Department: Support, Role: View Only.
</p>
  <img src="https://i.imgur.com/ujpOdKM.png" height="75%" width="100%" alt="agent one access"/>
<p>
  <img src="https://i.imgur.com/NcCP0v9.png" height="75%" width="100%" alt="agent two"/>
  <img src="https://i.imgur.com/aKTJ01A.png" height="75%" width="100%" alt="agent two access"/>
</p>
<h3 align="center">Configure Users (customers)</h3>
<br />
<p>
  Under Admin Panel > Go to "Users" -> Click "Add New"
  Add two end users named Ken & Karen. End users or customers, can create and view support tickets, access a knowledge base, and track the status of their issues through the customer portal. 
</p>
<p>
  Ken User:
</p>
  <img src="https://i.imgur.com/vbPd3uK.png" height="75%" width="100%" alt="user access"/>
<p>
  Do the same Step for Karen User.
</p>
<br />
<br />
<h3 align="center">Configure SLA</h3>
<br />
<p>
  Under the Admin Panel > Go to "Manage" section > Click on "SLA"
  1. Name: Sev-A           2. Sev-B          3. Sev-C
  1. Grace Period: 1-hour  2. 4-hour         3. 8-hour
  1. Schedule: 24/7        2. 24/7           3. M-F 8am-5pm + holidays
</p>
<p>
  <img src="https://i.imgur.com/6AAF3Ju.png" height="75%" width="100%" alt="sev one"/>
  <img src="https://i.imgur.com/izcD74X.png" height="75%" width="100%" alt="sev two"/>
  <img src="https://i.imgur.com/xKzdp7w.png" height="75%" width="100%" alt="sev three"/>
</p>
<br />
<br />
<h3 align="center">Configure Help Topics</h3>
<br />
<p>
  Under Admin Panel > Go to "Manage" > Click "Help Topics"
  Business Critical Outage (parent: Report a Problem) 
  Personal Computer Issues (parent: Report a Problem) 
  Equipment Request (parent: General Inquiry) 
  Password Reset (parent: Report a Problem) 
  Other (parent: General Inquiry)
</p>
<p>
  <img src="https://i.imgur.com/Xdhp63v.png" height="75%" width="100%" alt="business critical outage"/>
  <img src="https://i.imgur.com/3Y7k2o1.png" height="75%" width="100%" alt="personal computer issues"/>
  <img src="https://i.imgur.com/Z0eIGea.png" height="75%" width="100%" alt="equipment request"/>
  <img src="https://i.imgur.com/ndOdtTZ.png" height="75%" width="100%" alt="password reset"/>
</p>
<br />
<br />
<p>
  This now fully configures our osTicket and for a real-world help desk environment. I hope this guide was able to help clarify and assist you in setting up your osTicket. I recommended to practice triaging and solving tickets.
</p>
