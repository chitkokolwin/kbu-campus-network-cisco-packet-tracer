# OSPF Configuration

## Overview

OSPF (Open Shortest Path First) was implemented to provide dynamic routing between the Main Building and Lab Building.

Instead of manually adding routes, OSPF allows routers to automatically exchange network information and learn available paths.

## OSPF Design

- Routing Protocol: OSPF
- Process ID: 1
- Area: 0 (Single Area)
- Routers:
  - MB-Router
  - LB-Router

## Advertised Networks

### MB-Router

```
192.168.10.0/24
192.168.20.0/28
10.0.0.0/30
```

### LB-Router

```
192.168.30.0/24
192.168.40.0/27
10.0.0.0/30
```

## Verification

OSPF operation was verified using:

```
show ip ospf neighbor
```

Expected result:

- MB-Router and LB-Router establish a FULL OSPF neighbor relationship.

Routing information was checked using:

```
show ip route
```

Expected result:

- Remote networks appear as OSPF learned routes (O).
