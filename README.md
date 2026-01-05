# IT Home Lab - Week 1

## Lab Overview
Created a Windows Server 2022 lab to practice users, groups, and folder permissions, including a departmental folder simulation for HR and IT.

## Users <img width="1919" height="1022" alt="USERS" src="https://github.com/user-attachments/assets/d72bf9a1-be7e-487d-aafc-2b508a54026a" />

- User1 (GroupA / HR_Group)
- User2 (GroupB / IT_Group)
- User3 (no group)
- HR_User1, HR_User2 → HR_Group
- IT_User1, IT_User2 → IT_Group

## Groups <img width="1917" height="1014" alt="GROUPS" src="https://github.com/user-attachments/assets/ab330034-a9ab-4526-ba49-ea9c3450bd66" />

- GroupA, GroupB
- HR_Group, IT_Group

## Folders and Permissions <img width="1919" height="1021" alt="HR_FOLDER" src="https://github.com/user-attachments/assets/ccbb42bb-0e55-4bf4-8629-4f4ecafa21bd" />
 <img width="1919" height="1022" alt="IT_FOLDER " src="https://github.com/user-attachments/assets/4ca386a7-09fe-4aa8-ade3-4be583c3bd4b" />  <img width="1918" height="1022" alt="USERGROUPS_PERMISSION" src="https://github.com/user-attachments/assets/eccfc186-1d6d-49a6-8e04-4c87bf4e0f2f" />




- C:\LabFolder → Full Control for GroupA
- C:\HR_Folder → Full Control for HR_Group
- C:\IT_Folder → Full Control for IT_Group
- Tested access for each user to verify permissions

## Learning Outcomes
- Hands-on experience with Active Directory concepts
- Practiced creating users and groups
- Applied folder permissions to simulate role-based access control (RBAC)
- Simulated departmental access control for multiple groups

## Errors & Fixes
- Initially, non-group users could access C:\LabFolder due to inherited permissions → fixed by disabling inheritance and removing default Users group.
- Tested conflicting permissions (Allow vs Deny) to confirm Deny overrides Allow.
- Practiced restoring access after accidentally removing a user/group from folder permissions.
