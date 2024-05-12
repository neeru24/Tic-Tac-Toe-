# Tic-Tac-Toe Game
This is a simple web-based Tic-Tac-Toe game implemented using HTML, CSS, and JavaScript. It allows players to take turns placing their symbols (X or O) on a 3x3 grid. The game detects when a player has won or if the game ends in a draw.

 # Technologies Used
HTML: Provides the structure of the web page. <br>
CSS: Styles the elements and adds visual effects. <br>
JavaScript: Implements the game logic and interactivity. <br>

# Code Explanation
## HTML Structure:
The HTML provides the basic structure of the Tic-Tac-Toe game.<br>
It includes a container (div of class game) with nine buttons representing the game board. <br>
There's also a message container (<div of class msg-container hide) initially hidden, which will display the winner message and a "New Game" button when necessary. <br>
Two additional buttons outside the game container are provided for resetting the game and starting a new game. <br>
## CSS Styling:
CSS styles are applied to elements to define their appearance and layout. <br>
Styles define the background color, font, size, and other visual aspects of the game elements. <br>
Selectors like .box, .msg-container, .hide, .game, and button IDs (#reset-btn, #new-btn) are used to target specific elements and apply styling rules. <br>
## JavaScript Logic:
### Initialization:
Event listeners are assigned to each box/button to handle click events. <br>
Variables are initialized to keep track of the game state, such as turnO to determine whose turn it is. <br>
An array winPatterns is defined to represent the winning combinations on the game board. <br>
### Click Event Handling:
When a box/button is clicked, an event listener triggers a function. <br>
Depending on whose turn it is (turnO), the clicked box displays either an "X" or "O". <br>
The turnO variable is toggled to switch between players after each move. <br>
The clicked box is disabled to prevent further interaction. <br>
### Checking for a Winner: 
After each move, a function (checkWinner()) is called to determine if there's a winner. <br>
The function iterates through the winPatterns array to check if any of the winning combinations have been achieved. <br>
If a winning combination is found and all the boxes in that combination have the same value (either "X" or "O"), the game declares a winner and displays a message. <br>
The winning player's symbol is also displayed in the message. <br>
### Resetting the Game:
Two buttons (#reset-btn and #new-btn) allow players to reset the game or start a new game. <br>
When clicked, these buttons trigger a function (resetGame()) that resets the game state. <br>
The game board is cleared, all boxes/buttons are enabled, and the message container is hidden. <br>
### Overall Functionality:
The code provides the functionality for a basic Tic-Tac-Toe game where players can take turns placing their symbols ("X" or "O") on a 3x3 grid. <br>
It detects when a player has won or if the game ends in a draw. <br>
Players can reset the game or start a new game at any time using the provided buttons. <br>

## Contribution
Contributions are welcome! If you have any suggestions for improvements then feel free to submit a pull request.

![Tic-Tac-Toe Output](1. Tic-Tac-Toe)
