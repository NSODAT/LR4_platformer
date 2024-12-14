# 2D Game with Melee Attack

## Overview
This project is a 2D platformer game built using Python and Pygame. The game includes basic mechanics such as movement, jumping, platform collisions, and a melee attack system that allows the player to interact with enemies in close combat.

## Features
- **Player Movement**: Move left, right, and jump using keyboard inputs.
- **Gravity and Collisions**: Realistic gravity and platform collision handling.
- **Melee Attack**: Press the Spacebar to attack enemies within a specific range.
- **Enemy System**: Static enemies that can be removed upon attack.
- **Platform System**: Predefined platforms where the player can land and interact.

## Controls
- **Move Left**: Press `A`
- **Move Right**: Press `D`
- **Jump**: Press `W`
- **Melee Attack**: Press `Space`
- **Exit Game**: Close the window or press `Esc`

## Requirements
- Python 3.7 or higher
- Pygame library

## Installation
1. Clone the repository or download the source code.
2. Ensure Python is installed on your system.
3. Install Pygame using pip:
   ```bash
   pip install pygame
   ```
4. Run the game:
   ```bash
   python game.py
   ```

## Gameplay
- Move your character around the screen, jump between platforms, and avoid falling off.
- Use the melee attack to eliminate enemies within range. Enemies disappear upon successful attacks.

## Customization
### Adding Platforms
You can add new platforms by modifying the `platforms` list in the source code:
```python
platforms = [
    pygame.Rect(100, 500, 200, 10),
    pygame.Rect(400, 400, 200, 10),
    pygame.Rect(200, 300, 200, 10)
]
```
Each platform is defined as a rectangle with the format `pygame.Rect(x, y, width, height)`.

### Enemy Spawning
Enemies are represented as rectangles in the `objects` list. To add more enemies, update the list:
```python
objects = [
    pygame.Rect(200, 150, 50, 50),
    pygame.Rect(400, 300, 50, 50)
]
```
You can also modify the `spawn_enemy` function to dynamically add enemies.

### Attack Range
The melee attack range is determined by the `ATTACK_SIZE` variable. Modify this value to adjust the attack zone size:
```python
ATTACK_SIZE = 100
```

## Future Enhancements
- Add enemy AI to make enemies move or attack the player.
- Implement health and score systems.
- Include additional animations for jumping and attacking.
- Add levels with increasing difficulty.

## License
This project is licensed under the MIT License.

## Acknowledgments
- Developed using the [Pygame](https://www.pygame.org/) library.
- Thanks to the Python and Pygame communities for resources and tutorials.

