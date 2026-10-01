# IP Addressing Plan

## Overview

The KBU Campus Network uses IPv4 addressing to separate different departments and services into different network segments.

## Network Segments

| Segment | Network | Gateway |
|---|---|---|
| Main Building Administration | 192.168.10.0/24 | 192.168.10.1 |
| Server Network | 192.168.20.0/28 | 192.168.20.1 |
| Student Lab | 192.168.30.0/24 | 192.168.30.1 |
| IT Department | 192.168.40.0/27 | 192.168.40.1 |
| WAN Link | 10.0.0.0/30 | N/A |

## Router Interfaces

### MB-Router

| Interface | IP Address |
|---|---|
| Fa0/0 | 192.168.10.1 |
| Fa0/1 | 192.168.20.1 |
| Se0/0/0 | 10.0.0.1 |

### LB-Router

| Interface | IP Address |
|---|---|
| Fa0/0 | 192.168.30.1 |
| Fa0/1 | 192.168.40.1 |
| Se0/0/0 | 10.0.0.2 |
