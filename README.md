# Pong Game

This project is an interactive Ping Pong game that uses computer vision and hand tracking to create a unique gaming experience. Players use their hands as paddles to hit a virtual ball back and forth.

## Game Description

The game is a modern take on the classic Ping Pong. Instead of using physical paddles, players use their hands, which are tracked by a webcam. The game uses computer vision techniques to detect and track the players' hands in real-time.

### Key Features:

1. **Hand Tracking**: The game uses the `cvzone.HandTrackingModule` to detect and track the players' hands.
2. **Virtual Paddles**: Players' hands act as paddles. The game overlays virtual paddle images onto the detected hand positions.
3. **Dynamic Ball Movement**: A virtual ball moves across the screen, bouncing off the top and bottom edges.
4. **Collision Detection**: The game detects collisions between the ball and the paddles, changing the ball's direction accordingly.
5. **Scoring System**: The game keeps track of each player's score, incrementing it when the opponent misses the ball.
6. **Game Over Screen**: When a player misses the ball and it goes out of bounds, the game displays a "Game Over" screen with the final scores.
7. **Restart Functionality**: Players can restart the game by pressing the 'r' key.

## How to Play

1. Run the script and allow access to your webcam.
2. Two players stand in front of the webcam, one on each side.
3. Use your hands as paddles to hit the virtual ball back and forth.
4. The ball will speed up with each hit, increasing the difficulty.
5. Score points when your opponent misses the ball.
6. The game ends when the ball goes out of bounds on either side.
7. Press 'r' to restart the game at any time.
8. Press 'q' to quit the application.

## Technical Details

The game is built using Python and several key libraries:

- OpenCV (`cv2`): For image processing and display
- cvzone: For hand tracking and image overlay
- NumPy: For numerical operations

The game utilizes computer vision techniques to create an immersive and interactive gaming experience without the need for physical controllers.

## Setup and Requirements

### Prerequisites

1. Python 3.10 (the version used in the provided virtual environment)
2. Webcam

### Setup Steps

1. Activate the provided virtual environment:
   - On Windows:
     ```
     venv310\Scripts\activate
     ```
   - On macOS and Linux:
     ```
     source venv310/bin/activate
     ```

   You should see `(venv310)` appear at the beginning of your command line prompt, indicating that the virtual environment is active.

2. Verify that all required packages are installed:
   ```
   pip list
   ```
   You should see all necessary packages listed, including opencv-python, mediapipe, cvzone, numpy, and sympy.

### Running the Game

1. Ensure your virtual environment is activated (you should see `(venv310)` in your command prompt).

2. Run the main Python script:
   ```
   python main.py
   ```

3. Allow the application to access your webcam when prompted.

4. Position yourself (and another player, if playing with two people) in front of the webcam.

5. Use your hands as paddles to play the game!

### Controls

- Use your hands as paddles to hit the ball
- Press 'r' to restart the game
- Press 'q' to quit the application
