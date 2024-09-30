+++
title = "Simultaneous Opposite Cardinal Directions (SOCD) in rust 🦀 !"
date = 2024-09-22T12:34:13+02:00
draft = false
description = "Replicate the feature in certains keyboard to keep the last input sent"
tags = ['rust']
+++

[`🐙 Github source here 🐙`](https://github.com/RealColorDream/socd)


### You may have heard of new keyboards with short response time. Some of them have features that enable them to only response with the last input sent by the user.

### Here is a quick video that explain how SOCD works :

{{< youtube id=NPWfg0BjY2g loading=lazy alt="video that explain SOCD">}}

### So this quick script is meant to replicate the 'last input first' feature in certain keyboards.

### The script is written in Rust and uses the [`device_query crate`](https://crates.io/crates/device_query) crate to handle the users input.

### This script is simple, it reads the input from the user and if the user press two opposite directions at the same time, it will only keep the last input sent.

### I am currently considering to build a gui (graphic user interface) to keep the management of the user keymaps easy ✨
