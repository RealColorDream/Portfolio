+++
title = "Реализация игры Жизнь Конвея на Rust 🦀"
date = 2024-09-22T12:34:13+02:00
draft = false
description = "Простая реализация игры Жизнь Конвея, написанная на Rust."
tags = ['rust']
+++

## Простая реализация игры Жизнь Конвея, написанная на Rust.

[`🐙 Исходный код на Github здесь 🐙`](https://github.com/RealColorDream/game-of-life)

## Обзор игры

Игра Жизнь Конвея - это клеточный автомат, придуманный британским математиком Джоном Хортоном Конвеем в 1970 году. Это игра с нулевым количеством игроков, что означает, что ее развитие определяется начальным состоянием и не требует дальнейшего ввода. Игра состоит из сетки клеток, которые могут быть либо живыми, либо мертвыми, и она развивается через серию поколений на основе простых правил.

## Правила

Состояние каждой клетки в сетке обновляется одновременно на основе следующих правил:

1. **Выживание**: Живая клетка с двумя или тремя живыми соседями остается живой в следующем поколении.
2. **Смерть**: Живая клетка с менее чем двумя живыми соседями умирает (недостаток населения), и живая клетка с более чем тремя живыми соседями умирает (перенаселение).
3. **Рождение**: Мертвая клетка с точно тремя живыми соседями становится живой (размножение).

Эти правила создают динамическую систему, где простые начальные конфигурации могут привести к сложным поведением со временем.

### Для сборки и запуска этого проекта вам нужно установить следующее:

- Rust
- Cargo
- SDL2 (см. [руководство по установке крейта embedded-graphics](https://docs.rs/embedded-graphics-simulator/0.6.0/embedded_graphics_simulator/#setup))

### Игра реализована с использованием embedded-graphics и работает на 64x64 монохромном дисплее.

![Описание изображения](/Portfolio/img/game-of-life.png)

#### Клавиши управления:
- `Space` для паузы/возобновления игры
- `TAB` для сброса игры
- `Стрелки` для перемещения курсора
- `Enter` для переключения состояния клетки под курсором, когда игра на паузе
- `Escape` для выхода из игры
- `ЛКМ` для создания космического корабля в позиции курсора

Приятной игры!