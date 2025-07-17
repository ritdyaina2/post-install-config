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

- Secure and Customize Agent & User Access
- Define Ticket Visibility and Permissions
- Configure SLAs (Service Level Agreements)
- Set Up Help Topics
- Finalize System Behavior


<h2>Configuration Steps</h2>

<p>
STEP 1: Access the Admin and Agent Panels
  
- Admin Login URL:
http://localhost/osTicket/scp/login.php

- User Ticket Portal URL:
http://localhost/osTicket  

<img width="400" height="339" alt="59" src="https://github.com/user-attachments/assets/211646c8-7011-4074-b174-6c71910bb8ee" />


<img width="400" height="231" alt="60" src="https://github.com/user-attachments/assets/92a8d655-aef4-4389-b3e7-2504685fe004" /><


</p>
<p>
 STEP 2: Agent Panel vs Admin Panel
  
  - Admin Panel = Full control of osTicket
  - Agent Panel = Used by support agents to manage tickets
  

 <img width="400" height="482" alt="61" src="https://github.com/user-attachments/assets/5d54ced1-61fe-4bab-878d-300b5d270a32" /><

 <img width="400" height="168" alt="62" src="https://github.com/user-attachments/assets/5160fa5f-10c2-4103-97f2-4472d3fa53f5" /><


</p>
<p>
  
STEP 3: Configure Roles
Admin Panel → Agents → Roles
 - Click Add New Role
 - Name it Supreme Admin

<img width="420" height="73" alt="image" src="https://github.com/user-attachments/assets/378f8e1e-b891-4387-ae40-2cfad70022c5" /><

<img width="562" height="132" alt="image" src="https://github.com/user-attachments/assets/b7ecc17d-7115-4934-b68c-acd47d9a90ee" /><

<img width="460" height="109" alt="image" src="https://github.com/user-attachments/assets/22319dd4-8f79-4f2f-bd35-225a20b3e310" /><

<img width="322" height="165" alt="image" src="https://github.com/user-attachments/assets/b52f72e0-0b39-4d63-a32e-fc70b3b609a4" /><

<img width="430" height="344" alt="image" src="https://github.com/user-attachments/assets/c7f41a0c-b43f-4577-bdb8-14b021834650" /><

<img width="350" height="211" alt="image" src="https://github.com/user-attachments/assets/556815ac-872f-4038-8691-870c263eba66" /><

<img width="420" height="107" alt="image" src="https://github.com/user-attachments/assets/8ea6f715-b51d-485e-b5e1-a81d8df0986b" /><


STEP 4: Create Departments
Admin Panel → Agents → Departments
Add:
- SysAdmins
- Support

  <img width="420" height="73" alt="image" src="https://github.com/user-attachments/assets/07a3d1c3-956f-46bd-a34a-038811944c71" /><

<img width="450" height="123" alt="image" src="https://github.com/user-attachments/assets/6dfe9971-c096-44c6-b8b2-d0180f6da19c" /><

<img width="470" height="130" alt="image" src="https://github.com/user-attachments/assets/74f71c46-50b3-4d61-9d41-00d24f99df34" /><

<img width="417" height="163" alt="image" src="https://github.com/user-attachments/assets/ef026d21-7d83-482d-9ab4-f6c0f1853e14" /><

<img width="257" height="72" alt="image" src="https://github.com/user-attachments/assets/1b8f1c30-3d76-425a-94df-01938aac3001" /><

<img width="737" height="213" alt="image" src="https://github.com/user-attachments/assets/13c6159b-e55f-490b-aab1-af681a9a8b9c" /><


STEP 5: Create Teams
Admin Panel → Agents → Teams
 Add:
- Online Banking (pull agents from different departments)

<img width="420" height="73" alt="image" src="https://github.com/user-attachments/assets/378f8e1e-b891-4387-ae40-2cfad70022c5" />

<img width="460" height="379" alt="image" src="https://github.com/user-attachments/assets/c440471d-086d-4c44-8317-244fb1688066" /><

<img width="470" height="369" alt="image" src="https://github.com/user-attachments/assets/c6283d56-6536-4641-af31-07b8430520ad" /><

<img width="442" height="298" alt="image" src="https://github.com/user-attachments/assets/4948c556-1422-429f-9af9-974cb06fcb19" /><

<img width="298" height="48" alt="image" src="https://github.com/user-attachments/assets/5f72aa27-38e3-4fd6-bd08-cd47709984e8" /><

<img width="394" height="324" alt="Screenshot 2025-07-17 155159" src="https://github.com/user-attachments/assets/76e9cb62-6f28-44f6-b5de-a4d2d2499d15" />



 STEP 6: Allow Anyone to Create Tickets
- Admin Panel → Settings → User Settings
- UNcheck: “Require registration and login to create tickets”



STEP 7: Add Agents (Support Staff)
Admin Panel → Agents → Add New
 Add:
- Jane (Dept: SysAdmins)
- John (Dept: Support)
Assign them roles like Supreme Admin


STEP 8: Add Users (Customers)
Agent Panel → Users → Add New
 Add:
- Karen
- Ken


 STEP 9: Configure SLA (Service Level Agreements)
Admin Panel → Manage → SLA
 Add:
- Sev-A (1 hr, 24/7)
- Sev-B (4 hrs, 24/7)
- Sev-C (8 hrs, Business Hours)



 STEP 10: Create Help Topics
Admin Panel → Manage → Help Topics
 Add:
- Business Critical Outage
- Personal Computer Issues
- Equipment Request
- Password Reset
- Other
- 
<br />
