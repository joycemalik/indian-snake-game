# Cursor Snake - Apple Collector

This is a simple web-based game where the player controls a snake-like cursor to collect apples, while an AI snake also roams the screen. The game features smooth movement, wrap-around edges, and a dynamic speed increase.

## Features:

*   **Player-Controlled Snake:** Guide your snake with the mouse cursor.
*   **AI Opponent:** An autonomous snake collects apples on its own.
*   **Apple Collection:** Collect apples to increase your score and grow your snake.
*   **Dynamic Speed:** The game speed gradually increases over time, adding challenge.
*   **Wrap-Around Edges:** Both snakes and apples seamlessly transition from one side of the screen to the other.
*   **Visual Apple:** Apples are now represented by a graphical icon (a "Google Apple" style image) instead of a simple red circle.

## How to Play:

1.  Open `index.html` in your web browser.
2.  Move your mouse cursor around the screen. Your green snake's head will follow.
3.  Collect the apple icons to score points and make your snake grow longer.
4.  Currently, there is no collision detection with the red AI snake or the player's own body, focusing on the collection mechanic.

## Development Notes:

*   The game uses plain HTML, CSS, and JavaScript.
*   Canvas API is used for all game rendering.
*   The AI snake moves towards randomly generated targets.
*   The apple graphic is loaded from a public asset URL.

## Future Enhancements:

*   Add collision detection for player vs. AI snake, or player vs. self.
*   Implement different power-ups or obstacles.
*   Improve AI behavior.
*   Add a start/pause screen and game over conditions.
*   High score tracking.