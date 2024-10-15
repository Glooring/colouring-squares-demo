Iată un exemplu de fișier `README.txt` detaliat pentru proiectul tău *Colouring Squares*:

---

# Colouring Squares

**Colouring Squares** is a 2D puzzle game developed in Unity, where players color a grid of squares by using painter objects moving along the edges of the grid. The goal is to match the colors of all the grid cells with a predefined pattern, while overcoming obstacles and constraints.

## Features

- **Dynamic Grid Generation:** The game generates a grid based on the selected level, with customizable rows, columns, and spacing between squares.
- **Painter Mechanics:** Painters move across the grid, coloring the squares in their path. Players control the painters by clicking on them, making them move in specific directions.
- **Pattern Matching:** Each level has a predefined color pattern that players must replicate by coloring the squares correctly.
- **Levels and Difficulty Progression:** Multiple levels are available, each increasing in complexity, with unique patterns and painter setups.
- **Audio Management:** The game includes an audio system for playing various sound effects during gameplay (e.g., level completion, movement, interactions).
- **Grid Bounds Check:** Automatic out-of-bounds detection for painters, ensuring they are destroyed when moving outside the grid area.

## Gameplay

- Players interact with the game by clicking on painter objects positioned at the grid's edges.
- When a painter is clicked, it spawns a new painter that moves across the grid, coloring each square it touches.
- The goal is to match the color pattern displayed at the start of the level.
- The game features multiple levels, each with different patterns, grid sizes, and obstacles.

## Key Scripts

### 1. **AreaHandler.cs**
   - Detects collisions between objects and grid areas.
   - Used to destroy painters when they exit the grid bounds.

### 2. **AudioManager.cs**
   - Manages in-game sound effects, including playing, stopping, and overlapping sounds.
   - Utilizes a pool of audio sources to handle multiple sounds concurrently.

### 3. **BorderPatternFitter.cs**
   - Adjusts the size and position of a border object around a grid pattern to ensure proper fitting.
   - Dynamically calculates grid bounds based on the pattern size and spacing.

### 4. **Cell.cs**
   - Represents individual grid cells, each with a specific color.
   - Updates the cell's color based on the current painter's color when a painter passes through.
   - Integrates with the GridColors scriptable object for managing available colors.

### 5. **CheckOutOfBounds.cs**
   - Detects when painter objects move out of the grid bounds and destroys them to prevent unwanted behavior.

### 6. **DropdownDrawer.cs**
   - Custom property drawer for displaying dropdown menus in the Unity Inspector.
   - Enables easy selection of colors for grid cells from a predefined list of colors.

### 7. **GameManager.cs**
   - Handles game state management, including level progression, scoring, and unlocking levels.
   - Manages transitions between levels, score calculations, and UI updates.

### 8. **GridManager.cs**
   - Responsible for generating the grid and initializing cells based on the current level's settings.
   - Adjusts grid size, positions painters, and manages interactions between painters and grid cells.
   - Ensures grid color patterns are updated as players color the grid.

### 9. **Pattern.cs**
   - Defines the color pattern for each level, which players must match to complete the level.
   - Automatically generates the pattern based on the level's configuration.

### 10. **UIManager.cs**
   - Manages the game's user interface, including score display, level selection, and pause functionality.
   - Controls level completion panels, star ratings, and button visibility during gameplay.

## How to Play

1. Launch the game and select a level from the main menu.
2. Click on the painters at the bottom and right edges of the grid to make them move across the grid.
3. The goal is to color all the grid cells to match the level's predefined pattern.
4. Complete the level within the allowed moves to earn stars. The fewer moves, the more stars you earn.
5. Progress through the levels by unlocking them upon successful completion.

## Audio Management

The game includes an audio system for sound effects. Sound clips are played dynamically based on events such as:

- **Game Start:** Plays when a new level begins.
- **Level Completion:** Plays when the player successfully matches the pattern.
- **Painter Movement:** Plays while painters move across the grid.

## Grid Customization

The grid can be customized for each level using the following parameters:

- **Rows & Columns:** Define the number of rows and columns in the grid.
- **Spacing:** Adjust the spacing between grid cells.
- **Painter Colors:** Customize the colors used by painters when coloring the grid.

## Installation and Setup

1. Download and install [Unity](https://unity.com).
2. Clone or download the project from the repository.
3. Open the project in Unity.
4. In the Unity Editor, load the main scene and press Play to start the game.
5. Levels can be configured by modifying the level settings in the `GameManager.cs` and `Pattern.cs` scripts.

---

Let me know if you need further adjustments or details!