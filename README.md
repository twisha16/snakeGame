# Snake Arcade Game

A simple game of Snake in JS using Canvas

## Getting Started

Load snake.html in the browser

### Prerequisites

none

## Author

* **Twisha Shah**

## Next Steps

Few updates I would want to make to this game
* When creating the food, I don't check for the location being same as one occupied by any of the snake's squares. I would update that to check if it is already where the snake is and if it is, generate again and repeat the check.
* The wall collapse condition for the top and left wall is a bit off by 1 square, the right and down works fine. I never got to testing the collision with its own body because I never got that far in the game.
* I would want to have a start button instead of running the game loop on page load. For simplicity I just start the timer on window load for the game.
* Since this is a very simple game I did all the logic in one file. If I were to make it a bit more generic, I would move all the game logic into another module and import it into a main.js file and call methods on the imported module to inititialize the canvas with some params, set the timer for the game loop, set event handlers etc. This would also help with making some of those variables starting with "\_" private to functions/modules that care about them. Using import also required me to run a simple server to avoid running into the cors issues which seemed like an overkill.


## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details
