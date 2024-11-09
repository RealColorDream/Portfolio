+++
title = "Implémentation du jeu de la vie de Conway en Rust 🦀"
date = 2024-09-22T12:34:13+02:00
draft = false
description = "Une implémentation simple du jeu de la vie de Conway écrite en Rust."
tags = ['rust']
+++

## Une implémentation simple du jeu de la vie de Conway écrite en Rust.

[`🐙 Source Github ici 🐙`](https://github.com/RealColorDream/game-of-life)

## Présentation du jeu

Le jeu de la vie de Conway est un automate cellulaire inventé par le mathématicien britannique John Horton Conway en 1970. Il s'agit d'un jeu à zéro joueur, ce qui signifie que son évolution est déterminée par son état initial, sans nécessiter d'entrée supplémentaire. Le jeu se compose d'une grille de cellules qui peuvent être soit vivantes, soit mortes, et il évolue à travers une série de générations en fonction d'un ensemble de règles simples.

## Règles

L'état de chaque cellule de la grille est mis à jour simultanément en fonction des règles suivantes :

1. **Survie** : Une cellule vivante avec deux ou trois cellules vivantes voisines reste vivante à la génération suivante.
2. **Mort** : Une cellule vivante avec moins de deux cellules vivantes voisines meurt (sous-population), et une cellule vivante avec plus de trois cellules vivantes voisines meurt (surpopulation).
3. **Naissance** : Une cellule morte avec exactement trois cellules vivantes voisines devient vivante (reproduction).

Ces règles créent un système dynamique où des configurations initiales simples peuvent conduire à des comportements complexes au fil du temps.



### Pour construire et exécuter ce projet, vous devez avoir les éléments suivants installés :

- Rust
- Cargo
- SDL2 (référez-vous au [guide de la crate embedded-graphics](https://docs.rs/embedded-graphics-simulator/0.6.0/embedded_graphics_simulator/#setup) pour l'installation)


### Le jeu est implémenté à l'aide de embedded-graphics et s'exécute sur un écran monochrome 64x64.

![Description de l'image](/Portfolio/img/game-of-life.png)


#### Raccourcis clavier :
- `Espace` pour mettre en pause/démarrer le jeu
- `TAB` pour réinitialiser le jeu
- `Touches fléchées` pour déplacer le curseur
- `Entrée` pour basculer l'état de la cellule sous le curseur lorsque le jeu est en pause
- `Échap` pour quitter le jeu
- `Clic gauche` pour faire apparaître un vaisseau spatial à la position du curseur

Amusez-vous !
