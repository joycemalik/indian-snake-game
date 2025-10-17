# Cursor Snake

A simple, single-file web application featuring a smooth, cursor-following snake and an autonomous AI snake that gradually increases in speed over time. Both snakes wrap around the screen edges for continuous movement.

## How to Use

1.  **Save the file:** Save the provided `index.html` content into a file named `index.html` on your computer.
2.  **Open in browser:** Open the `index.html` file using any modern web browser (e.g., Chrome, Firefox, Safari).
3.  **Play:** Move your mouse cursor around the screen to control the green snake. Observe the red AI snake moving independently. The game speed will continuously increase, making the snakes move faster.

## Code Explanation

This project is a single-file HTML application (`index.html`) using vanilla JavaScript for all game logic and canvas rendering.

*   **HTML Structure:** A minimal HTML document containing a single `<canvas>` element, which serves as the drawing surface for the game.
*   **CSS Styling:** Basic CSS embedded in the `<style>` tags ensures the canvas fills the entire browser window and hides the default mouse cursor for a more immersive experience.
*   **JavaScript Logic:**
    *   **Game Loop (`gameLoop`):** Uses `requestAnimationFrame` for smooth, frame-rate independent animation. It calculates `deltaTime` to ensure consistent movement regardless of system performance.
    *   **Snakes:** Each snake is represented as an array of `{x, y}` objects (segments).
    *   **Player Snake Control:** The head of the player's green snake constantly moves towards the current mouse cursor position.
    *   **AI Snake Logic:** The red AI snake's head moves towards randomly generated target points on the screen. It picks a new target when it gets close to its current one or after a certain time has passed.
    *   **Smooth Following:** Each segment of both snakes smoothly interpolates its position towards the segment directly in front of it using a `FOLLOW_FACTOR`, creating a fluid, "spring-like" trailing effect.
    *   **Speed Increase:** The `gameSpeed` variable gradually increases based on the elapsed time since the game started, making the game progressively faster and more challenging.
    *   **Screen Wrap-Around:** Both snake heads and their segments handle screen boundaries by wrapping around to the opposite side, allowing continuous movement. This is implemented with shortest-path calculations to maintain visual smoothness.
    *   **Drawing:** The `draw` function clears the canvas and then renders each snake as a series of connected circles, with the head being slightly larger.

## License

This project is licensed under the MIT License.