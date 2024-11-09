+++
title = "Script de calcul CIDR en python (calculateur de sous-réseau) 🐍"
date = 2024-09-22T12:34:13+02:00
draft = false
description = "Un script simple pour calculer le CIDR d'une adresse IP donnée"
tags = ['python','réseau']
+++

[`🐙 Source Github ici 🐙`](https://github.com/RealColorDream/CIDR_script)
# Le calculateur CIDR est un script python simple pour calculer la notation CIDR d'une adresse IP.
## Il est conçu pour être aussi facile à utiliser que possible

## Utilisation :
```python
import CIDR as _

CIDR = _.CIDR("192.168.0.0", 24) # IP, nombre de sous-réseaux
print(CIDR) # par défaut, il affichera toutes les informations de cette IP
print(CIDR.first_IP_device())
```

## Méthodes :
```python
for method in dir(_.CIDR):
    if not method.startswith("__"):
        print(method)
# ['broadcast_IP', 'first_IP', 'first_IP_device', 'get_mask_Number', 'get_network_IP', 'last_IP', 'last_IP_device', 'number_of_IP', 'number_of_IP_device', 'parse_IP_to_int', 'parse_int_to_IP', 'parse_ip_to_list']
```
