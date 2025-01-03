+++
title = "Скрипт калькулятора CIDR на Python (калькулятор подсетей) 🐍"
date = 2024-09-22T12:34:13+02:00
draft = false
description = "Простой скрипт для вычисления CIDR заданного IP-адреса"
tags = ['python','network']
+++

[`🐙 Исходный код на Github здесь 🐙`](https://github.com/RealColorDream/CIDR_script)
# Калькулятор CIDR - это простой скрипт на Python для вычисления нотации CIDR IP-адреса.
## Он предназначен для максимально простого использования

## Использование:
```python
import CIDR as _

CIDR = _.CIDR("192.168.0.0", 24) # IP, количество подсетей
print(CIDR) # по умолчанию, он выведет всю информацию об этом IP
print(CIDR.first_IP_device())
```

## Методы:
```python
for method in dir(_.CIDR):
    if not method.startswith("__"):
        print(method)
# ['broadcast_IP', 'first_IP', 'first_IP_device', 'get_mask_Number', 'get_network_IP', 'last_IP', 'last_IP_device', 'number_of_IP', 'number_of_IP_device', 'parse_IP_to_int', 'parse_int_to_IP', 'parse_ip_to_list']
```
