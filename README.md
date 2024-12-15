# HC Pong AI

HC Pong AI is a simple Pong game implemented in Python using the Pygame library. This game features a basic AI that controls the right paddle, predicting the ball’s trajectory to intercept it. The game is intended to be a fun demonstration of AI's ability to predict and react to the ball’s movement in a classic Pong game setup.

## Features
- **Two-player gameplay**: One player controls the left paddle using the 'W' and 'S' keys.
- **AI-controlled opponent**: The right paddle is controlled by an AI that uses a simple prediction algorithm to move the paddle up or down.
- **Scoring system**: Each player scores by getting the ball past the opponent's paddle.
- **Ball prediction**: The AI predicts where the ball will land, adjusting its paddle position accordingly.

## Requirements
To run the game, you'll need Python 3 installed and the Pygame library.

1. **Install Python**:
   - Download Python from [python.org](https://www.python.org/downloads/).

2. **Install Pygame**:
   - Run the following command to install Pygame:
     ```bash
     pip install pygame
     ```

## How to Play
1. Clone or download the repository.
2. Run the game using Python:
   ```bash
   python pong.py

    Player Controls:
        'W': Move the left paddle up.
        'S': Move the left paddle down.

    The right paddle is controlled by the AI and will automatically move based on the ball's predicted path.

Game Flow

    The game starts with the ball at the center of the screen.
    The player controls the left paddle using the 'W' and 'S' keys.
    The AI controls the right paddle and uses its prediction algorithm to move.
    When the ball passes either paddle, the opponent scores a point.
    The first player to reach the set winning score (default 10) wins the game.
    After each point, the ball resets to the center, and the game continues.

AI Logic

The AI opponent uses a basic prediction algorithm to anticipate where the ball will be:

    Ball prediction: The predict_ball_location function simulates the ball’s movement and predicts where it will intersect with the AI's paddle.
    Paddle movement: The AI moves its paddle based on the predicted ball location, adjusting the paddle’s vertical position to intercept the ball.

The AI’s logic is not perfect and may sometimes miss the ball, but it provides a challenging experience for the player.
Customization

You can customize various aspects of the game:

    Paddle speed: Change the speed of both paddles by modifying the VEL attribute in the Paddle class.
    Ball speed: Adjust the maximum velocity of the ball by changing the MAX_VEL value in the Ball class.
    Winning score: Modify the WINNING_SCORE variable to change the number of points required to win the game.

How to Customize AI

    AI Difficulty: The AI's performance is influenced by the accuracy of its ball trajectory prediction. You can tweak the prediction logic for more challenging or easier gameplay.
    Paddle Size: You can change the size of the paddles by adjusting the PADDLE_WIDTH and PADDLE_HEIGHT variables.

File Structure

hc-pong-ai/
├── pong.py            # The main game script
└── README.md          # This file

License

This project is licensed under the MIT License. See the LICENSE file for more information.
Acknowledgments

    Pygame: https://www.pygame.org, a Python library used for creating video games.
    Inspiration: This project is inspired by the classic Pong game and the desire to implement a simple AI.


---

### Summary:

The repository name **`hc-pong-ai`** is short and directly reflects the purpose of the project. The `README.md` covers the essential details for setting up, running, and customizing the game, along with providing insights into the AI's mechanics. This should help anyone interested in your project understand its features and how to interact with it.
