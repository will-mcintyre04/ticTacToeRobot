# ticTacToeRobot

<div align = "center">
  <img src = "https://github.com/will-mcintyre04/ticTacToeRobot/assets/78566536/6b3e0489-df6f-4a4a-8577-e2567067794d" width = "600px"></img>
  
  <sub>Image showing the rack and pinion movement system (left) and drawing mechanism (right)</sub>
</div>

## Introduction
Collaborated in a multi-disciplinary, cross-functional team to build a robot using a LEGO EV3 brick, LEGO components, and a wide range of sensors that succesfuly plays Tic-Tac-Toe against a user. The bot builds, scans, and plays on the board while keeping track of high scores from the user, accepting I/O on highscore files and playing on different difficulty levels.

## Function

The robot communicates through a GUI that allows user input, data gathering, and score tracking.

A few of the tasks this robot can complete are:
- Receiving input on the difficulty level from the user and then drawing a 3 x 3 playing area with nominal values assigned to individual playing spots.
<p align="center">
  <img src = "https://github.com/will-mcintyre04/ticTacToeRobot/assets/78566536/438dae3e-48fc-4772-8471-71817ce2353a" width = "300px">
</p>

- Resetting to the default position (sensor/pen in the bottom left closest to the robot) and awaiting a move, signaled by the user by the touch sensor.
- Scanning the board using the color sensor and outputting to the user if they made an invalid play.
- Playing a spot based on difficulty level (easy will be a random valid spot, medium will have an equal chance to pick the best move or a random one, and hard mode will always make the best move).
- Looping through moves, user vs. robot until a terminal board condition is met (i.e., user or robot wins, or there is a tie).
- Ending the game and displaying to the user the result, as well as the cumulative score (1 for winning on easy, 2 for winning on medium, 3 for winning on hard), and the option to play again. These scores will also be recorded in a file that can be downloaded.
- If the user selects to end, exiting the code; if the user selects to play again, another board is created.

## Tools

- DC servo motors powering a rack and pinion system allowing full horizontal and vertical ROM over the playing area.
- Drawing mechanism that holds a pen and controls movement using a smaller servo motor.
- Linear motor encoders to measure distances and determine positioning.
- Velocity/resistance calculations to verify reset positions.
- Photoelectric colour sensor to correctly identify user play.
- Tactile sensors for user input and emergency stop.
- <a href = "https://www.neverstopbuilding.com/blog/minimax"> MiniMax Algorithm</a> implimentation to keep track of current board state and play the most optimal move given that state.

## Further Details
To view further detal about this project, see: [S8 Final Report 2022.pdf](https://1drv.ms/b/s!Are-DBXFp-MYvRyf3Eisvor8FYIC?e=WdYvac).
