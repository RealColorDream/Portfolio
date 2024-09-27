+++
title = "CIDR calculator script in python (subnet calculator) 🐍"
date = 2024-09-22T12:34:13+02:00
draft = false
description = "A simple script to calculate the CIDR of a given IP address"
tags = ['python','network']
+++
[`🐙 Github source here 🐙`](https://github.com/RealColorDream/CIDR_script)
# CIDR calculator is a simple python script to calculate the CIDR notation of an IP address.
## Its meant to be as easy as possible to use

## Usage:
```python
import CIDR as _

CIDR = _.CIDR("192.168.0.0", 24) # IP, subnet_numbers
print(CIDR) # by default, it will print all the information of this ip
print(CIDR.first_IP_device())
```

## Methods:
```python
for method in dir(_.CIDR):
    if not method.startswith("__"):
        print(method)
# ['broadcast_IP', 'first_IP', 'first_IP_device', 'get_mask_Number', 'get_network_IP', 'last_IP', 'last_IP_device', 'number_of_IP', 'number_of_IP_device', 'parse_IP_to_int', 'parse_int_to_IP', 'parse_ip_to_list']
```
