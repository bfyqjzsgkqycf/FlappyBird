## 1. Project Overview
This is a Java implementation of the classic Flappy Bird game. The game features a simple and intuitive interface, with various game elements such as a background, foreground, a bird, pipes, and clouds. It provides a game start interface, a game process, and a game over interface, allowing players to experience the fun of the Flappy Bird game.
## 2. Project Structure
- `app` Package:
  - `App.java`: The entry point of the game, which initializes and starts the game.
  - `Game.java`: The main game class that manages game components, window drawing, and game states.
- `component` Package:
  - `GameBackground.java`: Responsible for drawing the game background and handling its movement.
  - `GameForeground.java`: Manages the generation and drawing of clouds in the foreground.
  - `Bird.java`: Represents the bird in the game, handling its movement, flapping, and scoring.
  - `GameElementLayer.java`: Manages other game elements such as pipes.
  - `WelcomeAnimation.java`: Displays the game start interface.
  - `GameOverAnimation.java`: Displays the game over interface with scores.
- `util` Package:
  - `GameUtil.java`: A utility class that provides methods for loading images, calculating probabilities, and getting random numbers.
  - `Constant.java`: Defines various constants used in the game, such as window size, image paths, and game speeds.
## 3. Key Features
- **Multiple Game States**: The game has three states: `GAME_READY`, `GAME_START`, and `STATE_OVER`. Players can start the game by pressing the space bar on the start interface, and restart the game after it is over.
- **Random Cloud Generation**: Clouds are randomly generated in the foreground at a certain probability, adding visual richness to the game.
- **Double Buffering**: To avoid screen flickering caused by resource competition between threads, the game uses double buffering technology to draw game content.
## 4. How to Run
1. Ensure that you have the Java Development Kit (JDK) installed on your system.
2. Clone this repository to your local machine.
3. Navigate to the project directory in the terminal.
4. Compile the Java source files.
5. Run the `App` class to start the game.
## 5. Controls
**Space Bar**: In the `GAME_READY` state, pressing the space bar starts the game. In the `GAME_START` state, it makes the bird flap its wings. In the `STATE_OVER` state, it restarts the game.
## 6. Dependencies
The project mainly uses the Java standard library, and there are no external dependencies.
## 7. Future Improvements
Add more game elements, such as power - ups or obstacles.
Optimize the game performance and user experience.
Implement a ranking system to record and display high scores.
