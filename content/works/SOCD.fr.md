+++
title = "Directions Cardinalles Opposées Simultanées (DCOS) en rust 🦀 !"
date = 2024-09-22T12:34:13+02:00
draft = false
description = "Répliquer la fonctionnalité de certains claviers pour conserver la dernière entrée envoyée"
tags = ['rust']
+++

[`🐙 Source Github ici 🐙`](https://github.com/RealColorDream/socd)


### Vous avez peut-être entendu parler de nouveaux claviers avec un temps de réponse court. Certains d'entre eux ont des fonctionnalités qui leur permettent de répondre uniquement à la dernière entrée envoyée par l'utilisateur.

### Voici une courte vidéo qui explique comment fonctionne la DCOS :

{{< youtube id=NPWfg0BjY2g loading=lazy alt="vidéo qui explique la DCOS">}}

### Ce petit script est destiné à répliquer la fonctionnalité "dernière entrée en premier" de certains claviers.

### Le script est écrit en Rust et utilise la crate [`device_query`](https://crates.io/crates/device_query) pour gérer les entrées de l'utilisateur.

### Ce script est simple, il lit l'entrée de l'utilisateur et si l'utilisateur appuie sur deux directions opposées en même temps, il conservera uniquement la dernière entrée envoyée.

### Je suis actuellement en train de considérer la création d'une interface graphique utilisateur (GUI) pour faciliter la gestion des cartes clavier de l'utilisateur ✨
