<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>


<h2>Configuration Steps</h2>

<p>

The post configuration setup of the osTicket system is shown in this tutorial.
 
Okay, fantastic! osTicket has been implemented from scratch. We will now concentrate on some post-installation setup and perform some system administration. New roles will first be configured within the help desk. Go to the Admin panel-> Agents -> Roles to accomplish this. We'll establish the Supreme Admin. Enter the name of the new role after selecting "Add new role." <br />
Note: When you are in the Admin Panel at the top right will say Agent Panel and vice versa.
</p>

<p>
<img src="https://i.imgur.com/DoUc9L7.png" height="40%" width="40%" alt="Adding a new role"/>
</p>

<p>
Additionally, you can alter any roles’ permissions. In this instance, they will have full permissions because we are generating a Supreme Admin. Remember that an agent's permissions are determined by their role, thus not every agent will have unrestricted access. If you correctly followed the instructions, your screen should appear like this. As you can see, we were successful in setting up the role of "Supreme Admin".
</p>

<p>
<img src="https://i.imgur.com/kMXFZpC.png" height="40%" width="40%" alt="Surpreme Admin Role Established"/>
</p>

<p>
While in the Admin Panel go to the agents tab and click the "Departments" button. We will be able to establish a new department here. Depending on their designated job within the helpdesk, each Agent is assigned to a particular department. The "System Administrators" department will be established in this instance, and this is where the Supreme Admins will be identified. In the departments tab, you can configure additional particular parameters like SLAs, managers, and other email preferences.
</p>

<p>
<img src="https://i.imgur.com/xDEmbcI.png" height="40%" width="40%" alt="System Administrators Department"/>
</p>

<p>
We will establish a new team after configuring a new department. Teams give you the ability to assemble agents from several departments; for example, you may assemble an A team of the best technicians from a given department. You could, for instance, design a support topic that pertains to a product you make and assign it to a group of agents who are experts in that product. Go to Agents->Teams to form a team. In this example, a Level II support team will be created as a Level I support team has already been set up by default.
</p>

<p>
<img src="https://i.imgur.com/snBZtLl.png" height="40%" width="40%" alt="New Team"/>
</p>

<p>
Now that a new team has been established, we will create a new setting to enable anyone to create tickets. Admin Panel > Settings > User Settings <br />
Ensure that “require registration and login to create tickets” is turned off, this is important for any user to be able to create a ticket.
</p>

<p>
<img src="https://i.imgur.com/WraSq1M.png" height="40%" width="40%" alt="Allowing any user to create a ticket"/>
</p>

<p>
Now let's create some Agents. The help desk personnel who really work on solving tickets are known as agents. When tickets are routed to a department, agents are given a primary department and position. Agents may be granted access to departments other than their own, and depending on what department they are in, they may also have varied tasks. In the Agents tab, you may allocate Teams, Access, and Permissions. To begin, navigate to Admin Panel >> Agents >> Add new agent and create some agents of your choice.
</p>

<p>
<img src="https://i.imgur.com/Uv9SdIp.png" height="40%" width="40%" alt="Creating an agent"/>
</p>

<p>
<img src="https://i.imgur.com/5WzNfcB.png" height="40%" width="40%" alt="Agent acess"/>
</p>

<p>
<img src="https://i.imgur.com/68snH6Z.png" height="40%" width="40%" alt="Agent team"/>
</p>

<p>
Your agents should show like this once you click create.

<p>
<img src="https://i.imgur.com/whLsBrk.png" height="40%" width="40%" alt="New Agents"/>
</p>

<p>
We'll create users after creating some agents. Users are clients who create tickets when they encounter problems. A user can be recognized by their email address. Follow this guide to create a user. Agent Panel > Users > User Directory > Add User. After creating your user or users, your user directory should look like this:
</p>

<p>
<img src="https://i.imgur.com/gruInlK.png" height="40%" width="40%" alt="New users"/>
</p>

<p>
SLAs Plans specify how long the help desk is supposed to take to resolve a particular ticket. By navigating to Admin Panel >> Manage >> SLA Plans, SLA Plans can be generated. Every SLA has a schedule, and during that schedule, a grace period is allowed. SEV-A in this instance has a 24/7 and an hour-long grace period.
</p>

<p>
<img src="https://i.imgur.com/fuAvSbu.png" height="40%" width="40%" alt="Creating an SLA Plan"/>
</p>

<p>
Here is an example of how different SLA Plans can look
</p>

<p>
<img src="https://i.imgur.com/hMcTAmP.png" height="40%" width="40%" alt="Different SLAS"/>
</p>

<p>
Users can organize their tickets using the help topics. If consumers are unable to access mobile banking, we have created a help topic for them,"Business Critical Outage" is an example of this and can be viewed below.
</p>

<p>
<img src="https://i.imgur.com/goUdv13.png" height="40%" width="40%" alt="Help Topic"/>
</p>
