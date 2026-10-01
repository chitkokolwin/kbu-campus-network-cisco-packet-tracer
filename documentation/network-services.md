# Network Services

## Overview

The KBU Campus Network includes several internal services hosted in the Main Building Server Network.

These services provide users with essential network resources such as automatic IP assignment, name resolution, web access, email communication, and file sharing.

## Server Network

Network:

```
192.168.20.0/28
```

Gateway:

```
192.168.20.1
```

## Implemented Services

## DHCP Server

Purpose:

- Automatically assigns IP addresses to clients

Configuration:

- DHCP pool created for Administration users
- Gateway and DNS information provided automatically
- Client devices verified using DHCP mode

---

## DNS Server

Purpose:

- Provides hostname resolution inside the campus network

Configured records:

```
www.kbu.ac    → Web Server
mail.kbu.ac   → Email Server
ftp.kbu.ac    → FTP Server
dhcp.kbu.ac   → DHCP Server
```

---

## Web Server

Purpose:

- Hosts the campus intranet webpage

Verification:

- Accessed through a web browser using:

```
www.kbu.ac
```

---

## Email Server

Purpose:

- Provides internal email communication

Implemented:

- Email domain configuration
- User account creation
- Email sending test

---

## FTP Server

Purpose:

- Provides file sharing for IT users

Implemented:

- User authentication
- File upload testing
- FTP connectivity verification

---

## Wireless Network

Wireless access was added for Main Building staff.

Configuration:

- SSID: Kbu-Staff
- Security: WPA2-PSK
- Client connected using wireless adapter

---

## Verification

Services were tested using:

- DHCP IP assignment
- DNS hostname lookup
- Web browser access
- Email communication
- FTP file transfer
- Wireless connectivity test
