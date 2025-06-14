# 🐢 Turtle Crossing Game

A simple arcade-style crossing game built using Python’s Turtle graphics module. The objective is to help the turtle (player) cross the road and avoid oncoming cars. As the player progresses, the game gets faster and more challenging.

---

## 📸 Screenshot

![image](https://github.com/user-attachments/assets/282838f7-841a-4d01-8726-59e0add01100)


---

## 🎮 Game Description

- The player controls a turtle using the `Up` arrow key.
- Randomly generated cars travel horizontally across the screen from right to left.
- If the turtle reaches the top of the screen, the level increases and the game becomes faster.
- If the turtle collides with a car, the game ends with a "Game Over" message.

---

## 🧩 Project Structure

turtle-crossing-game/
│
├── main.py # Main game loop and event handling
├── player.py # Player class (the turtle)
├── car_manager.py # Car creation, movement, and speed logic
├── scoreboard.py # Display level and Game Over message
├── README.md # Project documentation
└── turtle_crossing.png # Optional screenshot for README


---

## 🐍 Technologies Used

- **Python 3.x**
- **Turtle Graphics** (standard Python library for GUI drawing)
- **time** and **random** modules

---

## 🚀 How to Run the Game

### Prerequisites:
Make sure you have Python installed. You can download it from [python.org](https://www.python.org/).

### Run the Game:

🧠 Game Logic Breakdown
main.py
Sets up the game window using Turtle's Screen().

Creates the player, cars, and scoreboard instances.

Listens for the player's input (Up key).

Repeatedly:

Generates cars at random intervals.

Moves all cars.

Checks for collision with cars.

Checks if the player reached the finish line (top of the screen).

Increases the level and game speed when the player succeeds.

player.py
Defines the Player class which:

Is shaped like a turtle.

Starts at the bottom of the screen.

Moves up with the go_up() method.

Checks whether it reached the finish line with is_at_finish_line().

Resets its position after each successful crossing.

car_manager.py
Handles all car logic:

Randomly generates cars using different colors and y-positions.

Moves all cars from right to left.

Increases speed as the player levels up.

scoreboard.py
Manages and displays the game state:

Displays the current level on the top-left.

Increments the level when the player succeeds.

Displays a "Game Over" message when the player collides with a car.

🎯 Game Features
🎮 Single Key Control: Just use the Up arrow to play.

🚗 Random Car Generation: Cars appear in random colors and vertical positions.

⚡ Dynamic Difficulty: Cars move faster with each level.

📉 Collision Detection: Game ends when the turtle collides with a car.

🧠 Object-Oriented Design: Cleanly organized using Python classes.

🔧 Future Improvements
Add left/right movement controls for more player freedom.

Introduce more lanes and difficulty settings.

Add sound effects using the winsound or pygame library.

Add a score counter based on time or crossings.

Save high scores using a file or database.

Improve visual aesthetics with custom car and turtle sprites.


