# Colouring Squares

## Demo

Play the demo on Vercel using the following link: [Colouring Squares - Demo](https://colouring-squares-demo.vercel.app/)

---

## How to Play

- **Objective**: The goal is to match the color pattern displayed at the start of each level by controlling painters that move along the grid edges.
- **Controls**: Click on the painters located at the edges of the grid to move them across the grid. Painters will color the squares as they pass over them.
- **Pattern Matching**: Players must color the grid to replicate the predefined pattern within a limited number of moves to complete the level.

---

## Features

1. **Dynamic Grid Generation**:
   - Each level generates a custom grid with adjustable rows, columns, and spacing between squares.
   
2. **Painter Mechanics**:
   - Players control painters that color squares as they move along the edges of the grid. Each painter leaves a trail of color, and players must strategically direct them to match the grid's pattern.
   
3. **Pattern Matching**:
   - Every level has a predefined pattern that players must match by coloring the squares. The difficulty increases as levels progress, with more complex patterns and fewer moves.

4. **Levels and Difficulty Progression**:
   - The game features multiple levels with progressively harder patterns and painter setups, adding complexity with each level.

5. **Grid Bounds Check**:
   - Painters are automatically destroyed if they move out of the grid's bounds, preventing unwanted behavior.

---

## Technologies and Concepts Used

1. **Unity Engine (2021.3 or higher)**:
   - The game is developed using Unity's 2D game development framework.

2. **Custom Grid Management**:
   - Dynamic grid generation for each level, adjusting grid size and cell arrangement based on level configurations.

3. **Scripted Game Logic**:
   - Key scripts handle player interaction, level progression, and pattern matching to ensure smooth gameplay.

4. **WebGL Deployment on Vercel**:
   - The game is deployed as a WebGL build for web-based gameplay.

---

## Future Improvements

- **Additional Levels**: Plan to introduce more levels with increasingly complex patterns.
- **New Obstacles and Constraints**: Adding new mechanics like obstacles and limited painter moves to further challenge players.
- **Mobile Optimization**: Refining the game for touch controls and smoother performance on mobile devices.

---

## License

The demo is for viewing purposes only.
