# Network Security - ACL Configuration

## Overview

Access Control Lists (ACLs) were implemented on the MB-Router to control traffic flow between different network segments.

The goal was to protect the Server Network while allowing authorized users and departments to access required resources.

## Security Policies

| Source Network | Destination | Action |
|---|---|---|
| Student Lab (192.168.30.0/24) | Server Network | Deny |
| Director PC (192.168.10.4) | All Networks | Permit |
| Administration Network | Server Network | Permit |
| IT Department (192.168.40.0/27) | Server Network | Permit |

## ACL Configuration

ACL Number:

```
10
```

Rules:

```
deny 192.168.30.0/24
permit host 192.168.10.4
permit 192.168.10.0/24
permit 192.168.40.0/27
```

## ACL Application

The ACL was applied to:

```
MB-Router FastEthernet0/1
```

Direction:

```
Outbound
```

This controls traffic going toward the Server Network.

## Verification

ACL operation was tested using:

```
show access-lists
```

Verification included:

- Confirming blocked Student Lab traffic
- Confirming allowed Director access
- Checking ACL match counters
