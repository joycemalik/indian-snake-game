# Cursor Snake - Apple Collector

This is a simple canvas-based game where the player controls a snake with their mouse, collecting apples to grow and score points, while avoiding or competing with an AI-controlled snake.

## Features:

*   **Player Control:** Your snake follows your cursor, providing direct and intuitive control.
*   **AI Opponent:** An autonomous AI snake navigates the canvas, following random targets.
*   **Dynamic Speed:** The game's overall speed gradually increases over time, adding challenge.
*   **Smooth Animations:** Physics-based segment following and `requestAnimationFrame` ensure fluid and responsive movement for both snakes.
*   **Screen Wrap-around:** Both snakes seamlessly pass through screen edges, reappearing on the opposite side.
*   **Apple Collection:** Collect randomly spawned apples to extend your snake's length.
*   **Gaming Points:** Earn points for each apple collected, displayed prominently on the screen.

## How to Play:

1.  Move your mouse cursor around the screen. Your green snake will follow.
2.  Guide your snake to collect the red apples that appear randomly.
3.  Each apple collected will increase your score and make your snake grow longer.
4.  Watch out for the red AI snake! While it doesn't directly harm you, it's also moving around.

## Technical Details:

*   Developed using plain HTML, CSS, and JavaScript.
*   Utilizes the Canvas API for all game rendering.
*   `requestAnimationFrame` is used for the main game loop, ensuring smooth animations synchronized with the browser's refresh rate.
*   Movement and following mechanics are based on delta time, ensuring consistent speed across different frame rates.
*   Collision detection is implemented for the player snake and apples.
*   The AI snake uses a simple random target selection mechanism, with targets changing periodically or upon reaching the current target.