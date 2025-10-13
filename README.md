# creating-a-backdoor-with-SET
creating a backdoor with SET - Ethical Hacking Techniques course

# AIM:
To Create a backdoor with Social Engineering Toolkit (SET)

## DESIGN STEPS:

### Step 1:

Install kali linux either in partition or virtual box or in live mode


### Step 2:

Investigate on the various categories of tools as follows:

### Step 3:

Open terminal and try execute some kali linux commands

### Architecture Diagram

```
+----------------+        +------------------------+        +----------------------+
| Attacker's PC  | -----> | SET (Credential        | -----> | Fake Login Page      |
| (Kali Linux)   |        | Harvester via Apache)  |        | (Hosted by SET)      |
+----------------+        +------------------------+        +----------------------+
       |                                                             |
       |                                                             v
       |   1. Configure SET with phishing site (e.g., Gmail clone)   |
       |                                                             |
       |                                                             v
       |                                                 +----------------------+
       |                                                 | Victim's Browser     |
       | <------------------------------------------------| Clicks Phishing Link|
       |                                                 +----------------------+
       |                                                             |
       |                                                             v
       |     2. Victim Enters Credentials → Sent to SET/Attacker     |
       |                                                             |
       |                                                             v
       |                                                 +----------------------+
       |                                                 | Credentials Captured |
       |                                                 | in Apache log/SET DB |
       |                                                 +----------------------+

```

## EXECUTION STEPS AND ITS OUTPUT:
Social Engineering attacks are the various cons used by the hackers to trick people into providing sensitive data to the attackers.

**Steps to Use SET for Phishing (Credential Harvester Attack Method)**

**1. Open terminal:**
```bash
sudo setoolkit

```

<img width="345" height="214" alt="Screenshot 2025-10-06 094432" src="https://github.com/user-attachments/assets/4707f51a-b233-4947-b863-a79ccf2de28b" />

**2.Navigate:**
```bash
1) Social-Engineering Attacks  
2) Website Attack Vectors  
3) Credential Harvester Attack Method  
```

<img width="346" height="239" alt="Screenshot 2025-10-06 094546" src="https://github.com/user-attachments/assets/12cc3ecc-3055-4514-b1cb-8a4c59490264" />
<br>
<img width="349" height="232" alt="Screenshot 2025-10-06 094617" src="https://github.com/user-attachments/assets/0f6ae51f-1a02-4c41-8d18-6f5fc346db9b" />
<br>
<img width="570" height="189" alt="Screenshot 2025-10-06 094641" src="https://github.com/user-attachments/assets/26ba4adb-9e03-4e2a-9cd4-197fc3e7d168" />

**4. Choose:**
```bash
2) Site Cloner
```

<img width="749" height="380" alt="Screenshot 2025-10-06 094727" src="https://github.com/user-attachments/assets/7d8c939f-4ae3-46bc-9f8e-d961ccdc6c90" />


**5. Enter the URL of the legitimate site ```(e.g., https://accounts.google.com)```**

<img width="943" height="279" alt="Screenshot 2025-10-06 095109" src="https://github.com/user-attachments/assets/ac59a8a8-868b-4b99-babd-b3bbc550206e" />


**6. Send the generated link to the victim.**

<img width="920" height="794" alt="Screenshot 2025-10-06 095308" src="https://github.com/user-attachments/assets/b9b4cde2-f713-4abe-a61d-7ad5d652e949" />



**7. Once the victim logs in → their credentials are stored in:**
```bash
/var/www/html/
```
<img width="944" height="465" alt="Screenshot 2025-10-06 095400" src="https://github.com/user-attachments/assets/59767083-f5c1-410c-a5a6-5ea5bf94ef18" />
<br>
<img width="948" height="427" alt="Screenshot 2025-10-06 095756" src="https://github.com/user-attachments/assets/e925d7e0-8a12-481e-9152-f523af2ae373" />




## RESULT:
The Social Engineering Toolkit (SET) is used to create backdoor is  examined successfully
