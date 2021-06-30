# Woodpecker

[Bird 2](https://bird.network.cz/) config for naive blackbox router RIB/FIB pressure test.

Test dataset:
- 300K BGP IPv4 unicast routes
- 80K OSPF IPv4 routes

## Usage

Usage example is provided for isolated secure lab environment only. Do not use this in production.

Tested on a CentOS 7 box with elrepo enabled:

```
yum install bird2
systemctl stop firewalld
systemctl stop bird
cd woodpecker
bird -c bird.conf -d
```
