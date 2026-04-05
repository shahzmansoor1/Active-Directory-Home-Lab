# Active-Directory-Home-Lab
In this lab, I create a domain controller, add users and security groups, then join a computer to the domain.


I start off by setting up a windows server 2022 virtual machine in virtual box

I then utilize **server manager** to add Active Directory Users and Computers while turning this server into a Domain Controller:

<img width="1018" height="792" alt="image" src="https://github.com/user-attachments/assets/aec7da64-e004-412d-91eb-6d3b021f54df" />


I create a name for my domain controller by the name of **smansoor.local**:

<img width="1018" height="851" alt="image" src="https://github.com/user-attachments/assets/229b996b-9e2b-481d-a62b-899c63888302" />


I follow this by adding an **Organizational Unit** by the name of **Edmonton Users** and add myself in it as a user:

<img width="168" height="56" alt="image" src="https://github.com/user-attachments/assets/7a4a4780-afc2-4b9b-9505-36dd890c9206" />


I then create a **security group** by the name of **Edmonton Security Users**:

<img width="191" height="92" alt="image" src="https://github.com/user-attachments/assets/6721d9df-6281-4722-bad1-acc004edfcd4" />


I then made myself a member of this security group:

<img width="401" height="347" alt="image" src="https://github.com/user-attachments/assets/cd2a5db0-f3b1-4a32-aa3e-5a9037ee0a57" />

I also configured the network on this computer so that I can add a comuter to th enetwork. I did this by manually adding an ip address and making hte default gateway the ip address of my router.

After these configurations, I decided to install windows 11 on a separate virtual machine instance.

AFter installation, I configured the ip address of that pc to be within the same subnet mask as the domain controller and made the default gateway the ip address of the domain controller

This allowed me to join that computer to he smansoor.local domain that I initially created:

<img width="1012" height="850" alt="image" src="https://github.com/user-attachments/assets/e7068bac-e656-4085-b804-0dc6ed49136d" />

This allows me to manage the computers, as well as the users and their permissions on the computer within my domain.
