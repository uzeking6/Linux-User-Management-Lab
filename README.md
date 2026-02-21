# 🔐 CYBERSECURITY ASSOCIATE – ASSIGNMENT 1  
## Linux User Management Lab (Kali Linux)

---

##  Lab Title
Linux User & Group Management with File Permissions

---

## 🎯 Objective

The objective of this lab is to demonstrate practical understanding of:

- Linux user creation and management
- Group creation and management
- File ownership configuration
- File permission settings using `chmod.`
- Ownership management using `chown.`
- Implementation of the Principle of Least Privilege

This lab simulates a real-world enterprise environment where different departments require different access control configurations.

---

## Scenario Overview

As the System Administrator for **TechCorp Solutions**, I was tasked with configuring user accounts and secure file access for two departments:

- Marketing Department (Private Individual Files)
- IT Department (Collaborative Shared File)

Each department required specific access control configurations to ensure proper data security and collaboration.

---

# 🟦 PART 1 – Marketing Department (Private Files)

### 📌 Requirements

- Create a group called `marketing.`
- Create 5 users:
  - alice_m
  - bob_m
  - carol_m
  - david_m
  - emma_m
- Add all users to the marketing group
- Create individual files for each user in:
  
  `/home/shared/marketing/.`

- Each file must:
  - Be owned by the respective user
  - Have permissions set to **700**
  - Be completely private (no group or others' access)

---

## Commands Executed

### Create Group
```bash
groupadd marketing
