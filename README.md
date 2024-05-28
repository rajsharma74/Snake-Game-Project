## Tile Class:

Represents a part of the snake or the food with x and y coordinates.
## Game Initialization:

SnakeGame(int boardWidth, int boardHeight): Initializes the game board and sets up the initial game state.
initGame(): Resets the game state including the snake's position, food's position, velocities, and game status.
## Drawing Components:

paintComponent(Graphics g): Calls draw(g) to render the game.
draw(Graphics g): Draws the grid lines, food, snake, and scores on the board. Also displays game over message if the game is over.
## Game Logic:

placeFood(): Places food in a random position on the board.
move(): Handles the snake's movement, checks for collisions, and updates the game state. If the game is over, it stops the game loop and updates the high score if the current score is higher.
Collision Detection:

collision(Tile tile1, Tile tile2): Checks if two tiles occupy the same position.
## Event Handling:

actionPerformed(ActionEvent e): Called by the Timer every 100 milliseconds to update the game state and repaint the board.
keyPressed(KeyEvent e): Handles key press events to change the snake's direction or restart the game if it is over.
keyTyped(KeyEvent e) and keyReleased(KeyEvent e): Not used but required by the KeyListener interface.
