# networkwalks-B082-week4-Penetration-Testing-Final-Project

<p align="center">
  <a href="#tech-stack">Tech Stack</a> •
  <a href="#networking">Networking</a> •
  <a href="#credits">Credits</a>
</p>


<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=rect&color=0:DC2626,100:7F1D1D&height=3&width=100%25" alt="divider" />
</p>

<h3 align="center" id="tech-stack">🛠️ Tech Stack</h3>
<p align="center">
  <img src="https://img.shields.io/badge/Cybersecurity-450A0A?style=for-the-badge&labelColor=DC2626&logo=hackthebox&logoColor=white" alt="Cybersecurity" />
  <img src="https://img.shields.io/badge/Windows-450A0A?style=for-the-badge&labelColor=000000&logo=windows&logoColor=white" alt="Windows" />
<img src="https://img.shields.io/badge/Penetration%20Testing-450A0A?style=for-the-badge&labelColor=DC2626&logo=kalilinux&logoColor=white" alt="Penetration Testing" />
</p>

<h3 align="center" id="networking">🌐 Networking</h3>
<p align="center">
  <img src="https://img.shields.io/badge/Cisco-450A0A?style=for-the-badge&labelColor=1BA0D7&logo=cisco&logoColor=white" alt="Cisco" />
  <img src="https://img.shields.io/badge/Networking-450A0A?style=for-the-badge&labelColor=EF4444&logo=wireguard&logoColor=white" alt="Networking" />
  <img src="https://img.shields.io/badge/Isolated%20Networking-450A0A?style=for-the-badge&labelColor=991B1B&logo=protonvpn&logoColor=white" alt="Isolated Networking" />
</p>

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=rect&color=0:F87171,100:7F1D1D&height=3&width=100%25" alt="divider" />
</p>

<h3 align="center" id="credits">🤝 Credits</h3>
<p align="center">
  <img src="https://img.shields.io/badge/Program-Network%20Walks-450A0A?style=for-the-badge&labelColor=B91C1C" alt="Network Walks" />
  <img src="https://img.shields.io/badge/Instructor-Waqas%20Karim%20(CCIE)-450A0A?style=for-the-badge&labelColor=DC2626&logo=cisco&logoColor=white" alt="Waqas Karim CCIE" />
  <img src="https://img.shields.io/badge/By-Asher%20Maxwell-450A0A?style=for-the-badge&labelColor=E11D48&logo=github&logoColor=white" alt="Asher Maxwell" />
</p>

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=rect&color=0:7F1D1D,100:DC2626&height=3&width=100%25" alt="divider" />
</p>


# 📌 Overview
-- Insert overview --

## 🖥️ Lab Environment

| Component          | Configuration         |
| :----------------- | :-------------------- |
| **Host OS**        | Windows               |
| **Attack Machine** | Windows 11            |
| **Project**        | Week 4                |
| **Focus**          | Penetration Testing   |
| **Primary Tool**   |  |
| **GUI Tool**       |                 |
| **Program**        | Network Walks         |


## General Steps
1. Conduct Reconnaissance

# Milestone 1

## 1.  Conduct Reconnaissance


### WHOIS Enumeration

### Domain Information

| Attribute | Value |
|---|---|
| **Domain** | `medirozahospital.com` |
| **Registry Domain ID** | `3132326963_DOMAIN_COM-VRSN` |
| **Creation Date** | `2026-08-14 20:51:24 UTC` |
| **Expiration Date** | `2027-08-14 20:51:24 UTC` |
| **Domain Status** | `clientTransferProhibited` |
| **DNSSEC** | Unsigned |

### Registrar Information

| Attribute | Value |
|---|---|
| **Registrar** | NameCheap, Inc. |
| **IANA ID** | `1068` |
| **WHOIS Server** | `whois.namecheap.com` |
| **Registrar URL** | `http://www.namecheap.com` |
| **Abuse Email** | `abuse@namecheap.com` |
| **Abuse Phone** | `+1.6613102107` |

### DNS Information

| Record | Value |
|---|---|
| **Name Server 1** | `dns1.namecheaphosting.com` |
| **Name Server 2** | `dns2.namecheaphosting.com` |

### Privacy / Registrant Information

| Attribute | Value |
|---|---|
| **Registrant** | Redacted for Privacy Purposes |
| **Organization** | Withheld for Privacy LLC |
| **City** | Lewes |
| **State/Province** | Delaware |
| **Country** | US |

> **Note:** Registrant, administrative, and technical contact information is protected by the registrar's privacy service.


## 2. WhatWeb Enumeration

| Attribute | HTTP | HTTPS |
|---|---|---|
| **URL** | `http://medirozahospital.com` | `https://medirozahospital.com` |
| **Status** | `200 OK` | `200 OK` |
| **Country** | United States (`US`) | United States (`US`) |
| **IP Address** | `199.188.201.16` | `199.188.201.16` |
| **HTTP Server** | OpenResty | OpenResty |
| **Server Version** | `1.31.1.1` | `1.31.1.1` |
| **HTML** | HTML5 | HTML5 |
| **Script** | Detected | Detected |
| **Page Title** | `One moment, please...` | `One moment, please...` |
| **Uncommon Headers** | `cf-edge-cache` | `cf-edge-cache` |


## 3. NSLookup Enumeration

| Attribute | Result |
|---|---|
| **DNS Server** | `8.8.8.8` |
| **DNS Server Address** | `8.8.8.8#53` |
| **Response Type** | Non-authoritative answer |
| **Domain** | `medirozahospital.com` |
| **Resolved IP Address** | `199.188.201.16` |


## 4. cURL Enumeration

| Header | Value |
|---|---|
| **HTTP Version / Status** | `HTTP/2 200 OK` |
| **Server** | `openresty/1.31.1.1` |
| **Date** | `Wed, 09 Sep 2026 01:02:30 GMT` |
| **Content-Type** | `text/html` |
| **Cache-Control** | `private, no-cache, no-store, must-revalidate, max-age=0` |
| **CF-Edge-Cache** | `no-cache` |

## 5. WAFW00F Enumeration

| Attribute | Result |
|---|---|
| **Target** | `https://medirozahospital.com` |
| **WAF Detected** | LiteSpeed WAF |
| **WAF Provider** | LiteSpeed Technologies |
| **Requests Made** | `2` |
| **Detection Status** | WAF Detected |


## 6. Search for `Robots.txt` 
Robots.txt file is a file that can be considered important. This file essentially tells robots/web scappers what pages or areas they can access and what they can't. Seeing this file can reveal vulnurabilities of a web application.

**We check the robots.txt file**
`curl https://medirozahospital.com/robots.txt`
`output`
<img width="418" height="153" alt="image" src="https://github.com/user-attachments/assets/b2747273-095f-472e-843a-eec49d26183e" />


# Step 2 - Route to the Login Page

<img width="1918" height="974" alt="image" src="https://github.com/user-attachments/assets/e8be486b-f72e-4976-bacc-3690511c399f" />

# Step 3 - Testing Input Validation 

#### Test 1
<img width="404" height="458" alt="image" src="https://github.com/user-attachments/assets/b8960a0c-ccce-487d-94b7-ec436d9ccffa" />

#### Test 2
<img width="401" height="449" alt="image" src="https://github.com/user-attachments/assets/370b8274-24de-4344-bc1a-88f0e1f75585" />

* We realize that in the first try it says username does not exist.
* Then in test 2, the error message changes to password is incorrect.
* This clearly shows that their is a dedicated user by the name of admin in the system.

# Step 4 - Check for SQL Injection Vulnurabilities

<img width="406" height="522" alt="image" src="https://github.com/user-attachments/assets/9ea9e21f-be32-4ca3-984c-bdd3ccfa81ee" />


<img width="397" height="522" alt="image" src="https://github.com/user-attachments/assets/417a21b8-35c0-419d-915f-305cacf10fea" />

</br>
<img width="1561" height="619" alt="image" src="https://github.com/user-attachments/assets/ebd42027-af69-4a5a-b86b-55c6ca7431f3" />

# Step Download Reports








