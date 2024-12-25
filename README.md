# Maze Adventure Game

## Introduction
This project is an Arduino-based maze adventure game. Players navigate through a maze using a joystick to find treasures and reach the exit while avoiding traps. The game uses various hardware components, including an LED matrix, LCD display, buttons, and a buzzer.

## Features
- **8×16 Maze Navigation**: The maze is displayed on an 8×8 LED matrix, with player movement handled dynamically across the entire 8×16 grid.
- **Dynamic Objects**:
  - **Walls (1)**: Static obstacles in the maze.
  - **Treasure (2)**: Collectible items that the player must find.
  - **Exit (3)**: The goal of the maze. Reach it to win.
  - **Traps (4)**: Hazards that end the game if triggered.
- **Interactive Controls**:
  - **Joystick**: Controls player movement.
  - **Red Button**: Displays game status and collected items.
  - **White Button**: Restarts the game.
- **Flashing Effects**: Items like treasure, traps, and exit blink to enhance visual feedback.
- **Non-blocking Buzzer Alerts**: Provides audio feedback for player actions.
- **Dynamic Maze Generation**: The game can randomly select from predefined maze layouts.

## Hardware Components
- **LCD (16×2)**: Displays game status messages (e.g., "YOU WIN!" or "GAME OVER").
- **LED Matrix (8×8)**: Visualizes the maze and player movement.
- **Joystick Module**: Enables directional control and button press detection.
- **Buzzer**: Emits sound feedback for key events.
- **Push Buttons**: Red and white buttons for interaction.

## Gameplay
### Objective
- Collect all treasures in the maze.
- Navigate to the exit to win the game.
- Avoid traps to prevent losing the game.

### Controls
- Move the player using the joystick.
- Use the red button to check collected items.
- Press the white button to restart the game.

### Game States
- **Ongoing**: Navigate the maze and interact with objects.
- **Victory**: Display "YOU WIN!" when the player reaches the exit.
- **Game Over**: Display "GAME OVER!" when the player steps on a trap.

## How It Works
- **Maze Representation**: The maze is stored as an 8×16 grid, where each cell represents a specific type of object (wall, treasure, exit, trap, or empty space).
- **LED Refreshing**: The LED matrix refreshes multiple times per second to reduce flickering and display smooth animations.
- **Player Interaction**: The player's position updates dynamically based on joystick input, with collision detection for walls and traps.
- **Random Mazes**: At the start of each game, a random maze layout is selected from predefined options.

## Future Improvements
- Add multiple difficulty levels with more complex mazes.
- Implement a scoring system based on the time taken and treasures collected.
- Expand the maze to larger grids with scrolling functionality.
- Add multiplayer support for cooperative or competitive gameplay.

Feel free to clone this repository and experiment with the code to customize the maze and gameplay mechanics!


// 中文说明
# 迷宫冒险游戏



＃＃ 介绍

本项目是一款基于Arduino的迷宫冒险游戏。玩家使用操纵杆在迷宫中导航，寻找宝藏并到达出口，同时避开陷阱。游戏使用了各种硬件组件，包括 LED 矩阵、LCD 显示屏、按钮和蜂鸣器。



＃＃ 特点

- **8×16 迷宫导航**：迷宫显示在 8×8 LED 矩阵上，玩家在整个 8×16 网格上的移动动态处理。

- **动态对象**：

  - **墙壁 (1)**：迷宫中的静态障碍物。

  - **宝藏 (2)**：玩家必须找到的收藏品。

  - **出口 (3)**：迷宫的目标。达到目标即可获胜。

  - **陷阱 (4)**：触发后会结束游戏的危险。

- **交互式控制**：

  - **操纵杆**：控制玩家移动。

  - **红色按钮**：显示游戏状态和收集的物品。

  - **白色按钮**：重新启动游戏。

- **闪烁效果**：宝藏、陷阱和出口闪烁等物品可增强视觉反馈。

- **非阻塞蜂鸣器警报**：为玩家操作提供音频反馈。

- **动态迷宫生成**：游戏可以从预定义的迷宫布局中随机选择。



## 硬件组件

- **LCD (16×2)**：显示游戏状态消息（例如，“你赢了！”或“游戏结束”）。

- **LED 矩阵 (8×8)**：可视化迷宫和玩家运动。

- **操纵杆模块**：启用方向控制和按钮按下检测。

- **蜂鸣器**：针对关键事件发出声音反馈。

- **按钮**：用于交互的红色和白色按钮。



## 游戏玩法

＃＃＃ 客观的

- 收集迷宫中的所有宝藏。

- 导航至出口以赢得游戏。

- 避免陷阱以防止输掉游戏。



### 控制

- 使用操纵杆移动玩家。

- 使用红色按钮检查收集的物品。

- 按白色按钮重新开始游戏。



### 游戏状态

- **正在进行**：在迷宫中导航并与物体互动。

- **胜利**：显示“你赢了！”当玩家到达出口时。

- **游戏结束**：显示“游戏结束！”当玩家踩到陷阱时。



## 实现游戏的机制

- **迷宫表示**：迷宫存储为 8×16 网格，其中每个单元格代表特定类型的对象（墙壁、宝藏、出口、陷阱或空白空间）。

- **LED 刷新**：LED 矩阵每秒刷新多次，以减少闪烁并显示流畅的动画。

- **玩家交互**：玩家的位置根据操纵杆输入动态更新，并对墙壁和陷阱进行碰撞检测。

- **随机迷宫**：在每场游戏开始时，都会从预定义的选项中选择随机迷宫布局。



## 未来的改进

- 添加多个难度级别和更复杂的迷宫。

- 根据所用时间和收集的宝藏实施评分系统。

- 通过滚动功能将迷宫扩展到更大的网格。

- 添加对合作或竞争游戏的多人支持。



请随意克隆此存储库并尝试使用代码来自定义迷宫和游戏机制！