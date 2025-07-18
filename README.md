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

- Admin Panel → Agents → Teams
 Add:
- Online Banking (pull agents from different departments)

<img width="420" height="73" alt="image" src="https://github.com/user-attachments/assets/378f8e1e-b891-4387-ae40-2cfad70022c5" /><

<img width="460" height="379" alt="image" src="https://github.com/user-attachments/assets/c440471d-086d-4c44-8317-244fb1688066" /><

<img width="470" height="369" alt="image" src="https://github.com/user-attachments/assets/c6283d56-6536-4641-af31-07b8430520ad" /><

<img width="442" height="298" alt="image" src="https://github.com/user-attachments/assets/4948c556-1422-429f-9af9-974cb06fcb19" /><

<img width="298" height="48" alt="image" src="https://github.com/user-attachments/assets/5f72aa27-38e3-4fd6-bd08-cd47709984e8" /><

<img width="394" height="324" alt="Screenshot 2025-07-17 155159" src="https://github.com/user-attachments/assets/76e9cb62-6f28-44f6-b5de-a4d2d2499d15" />-



 STEP 6: Allow Anyone to Create Tickets
- Admin Panel → Settings → User Settings
- UNcheck: “Require registration and login to create tickets”
  
<img width="420" height="73" alt="image" src="https://github.com/user-attachments/assets/378f8e1e-b891-4387-ae40-2cfad70022c5" /><

<img width="430" height="366" alt="image" src="https://github.com/user-attachments/assets/1518d90c-955d-44b8-9c96-bc8a5b6aff07" />


STEP 7: Add Agents (Support Staff)

Admin Panel → Agents → Add New

 Add:
- Jane (Dept: SysAdmins)
- John (Dept: Support)
Assign them roles like Supreme Admin

<img width="420" height="73" alt="image" src="https://github.com/user-attachments/assets/378f8e1e-b891-4387-ae40-2cfad70022c5" /><

<img width="460" height="124" alt="image" src="https://github.com/user-attachments/assets/31414990-fce3-4835-9daa-1ede20a38d71" /><

<img width="460" height="231" alt="image" src="https://github.com/user-attachments/assets/5f5abacb-cd7c-4002-89c3-dddfa6ef3c0a" /><

<img width="462" height="285" alt="image" src="https://github.com/user-attachments/assets/cdf3fd36-c737-448b-bdf4-83389170e032" /><

<img width="460" height="301" alt="image" src="https://github.com/user-attachments/assets/339a1ea5-3cd8-45a4-9206-71c9603837d8" /><

<img width="430" height="251" alt="image" src="https://github.com/user-attachments/assets/d76bdd1c-345d-4cfd-8a9b-1419bd4cd26b" /><

<img width="430" height="240" alt="image" src="https://github.com/user-attachments/assets/a1ba1d7e-9dc2-44a6-b6ff-3371fdecb02f" /><



<img width="460" height="457" alt="image" src="https://github.com/user-attachments/assets/d505dca6-0e0f-41bc-b285-730ebac86a03" /><

<img width="596" height="169" alt="image" src="https://github.com/user-attachments/assets/9bf009b7-2d8c-483c-8f34-7101882813d1" /><

<img width="360" height="132" alt="image" src="https://github.com/user-attachments/assets/a3a2931d-bad9-4d1f-8584-8495782f7a44" /><

<img width="430" height="202" alt="83" src="https://github.com/user-attachments/assets/88f3c805-c44c-4f7d-8c3b-49e6b69ad28a" /><


<img width="460" height="243" alt="image" src="https://github.com/user-attachments/assets/49f9becf-1e5d-4780-a23a-a5d8d14ffb18" /><

<img width="430" height="375" alt="image" src="https://github.com/user-attachments/assets/3cd5b778-5f0a-4418-bf68-dc74aabc1302" /><

<img width="434" height="271" alt="image" src="https://github.com/user-attachments/assets/359d5ebe-5076-41d5-a361-472b739ed1d3" /><

<img width="460" height="202" alt="image" src="https://github.com/user-attachments/assets/4b99fd7e-19b8-4a6e-86eb-d408784ff2c2" /><


STEP 8: Add Users (Customers)
Agent Panel → Users → Add New
 Add:
- Karen
- Ken

<img width="313" height="78" alt="image" src="https://github.com/user-attachments/assets/064187b6-4f0f-4830-a883-55db6bb317dc" /><

<img width="460" height="147" alt="image" src="https://github.com/user-attachments/assets/f8543938-42ba-46fd-8b77-2e72faf5a3f6" /><

<img width="430" height="251" alt="image" src="https://github.com/user-attachments/assets/0044b1b7-8aa5-4e4e-a0fc-b984586331b1" /><


 STEP 9: Configure SLA (Service Level Agreements)
Admin Panel → Manage → SLA
 Add:
- Sev-A (1 hr, 24/7)
- Sev-B (4 hrs, 24/7)
- Sev-C (8 hrs, Business Hours)
  
<img width="420" height="73" alt="image" src="https://github.com/user-attachments/assets/378f8e1e-b891-4387-ae40-2cfad70022c5" /><

<img width="460" height="67" alt="image" src="https://github.com/user-attachments/assets/07f90729-9c0a-4974-81f5-f703b67f4f45" /><

<img width="430" height="338" alt="image" src="https://github.com/user-attachments/assets/e1f71c9c-3c32-4cab-95eb-7199f9e91a77" /><

<img width="430" height="333" alt="image" src="https://github.com/user-attachments/assets/8400bc1b-c929-4a68-963e-0d1a95a04603" /><

<img width="430" height="337" alt="image" src="https://github.com/user-attachments/assets/4a64a8bb-3380-4d44-b277-352209fa544c" /><


 STEP 10: Create Help Topics
Admin Panel → Manage → Help Topics
 Add:
- Business Critical Outage
- Personal Computer Issues
- Equipment Request
- Password Reset
- Other
  
 <img width="420" height="73" alt="image" src="https://github.com/user-attachments/assets/378f8e1e-b891-4387-ae40-2cfad70022c5" /><

<img width="460" height="65" alt="image" src="https://github.com/user-attachments/assets/6ed10d62-4d2f-4634-b382-055c9d51b19e" /><

<img width="430" height="327" alt="image" src="https://github.com/user-attachments/assets/23b8942d-d9b8-4c60-8095-e11e8eb0763d" /><

<img width="430" height="313" alt="image" src="https://github.com/user-attachments/assets/ed951b11-5b1b-47d4-9293-31c69d7d6a4e" /><

<img width="430" height="316" alt="image" src="https://github.com/user-attachments/assets/654633d7-572f-4c38-b8fa-a4b1e4c43f8c" /><

<img width="430" height="307" alt="image" src="https://github.com/user-attachments/assets/aaae127d-d0e5-4f0c-891d-c33d8e0ae9d9" /><

<img width="430" height="306" alt="image" src="https://github.com/user-attachments/assets/f4be6bc7-b2de-447a-8028-4e50b9505b74" /><

<img width="430" height="250" alt="98" src="https://github.com/user-attachments/assets/2a03d736-ed87-4603-8565-97a955c729e2" /><

<br />
