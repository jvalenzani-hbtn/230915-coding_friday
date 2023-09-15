# Text-Based Minesweeper Game

In this exercise, you will create a simplified version of the classic single-player computer game, Minesweeper. Your task is to implement a text-based version of this game that operates in the console or terminal.

## Focus on:

- User i/o
- Multi dimensional arrays
- OOP
- Game logic

## Language

This exercise is intended to be done using Python or JavaScript (Node.js), but you're free to use whatever you like. 

## Requirements:

1. **Grid Representation**:
   - Create an NxN grid where the user can specify the value of N.
   - The grid should contain B mines (or bombs) hidden randomly across the grid.
   - The user should be able to specify the value of B but ensure B ≤ N².
   
2. **Cell Values**:
   - Each cell in the grid can be a bomb, a blank space, or a number.
   - The number in a cell represents the count of bombs in the eight surrounding cells.

3. **Gameplay**:
   - The user can uncover a cell to reveal its content.
   - If the user uncovers a bomb, the game ends, and the user loses.
   - If the user uncovers a number, that number becomes visible, and the turn ends.
   - If the user uncovers a blank cell, all adjacent blank cells (up to and including the surrounding numeric cells) should be revealed.
   - The user wins if all non-bomb cells are uncovered without uncovering a bomb.

4. **Flagging**:
   - Allow the user to flag cells that they suspect contain bombs.
   - Flagging a cell should not affect the gameplay other than preventing the user from uncovering that cell accidentally.

#### Instructions:

1. **Setup**:
   - Choose either Python or JavaScript for this exercise.
   - Create a new file named `minesweeper.py` (for Python) or `minesweeper.js` (for JavaScript).

2. **Grid Initialization**:
   - Implement a function to initialize the NxN grid with B bombs placed randomly.
   - Implement a function to calculate the number in each cell based on the surrounding bombs.

3. **User Interaction**:
   - Implement a function to handle user inputs for uncovering or flagging a cell.
   - The user should input the coordinates of the cell they want to uncover or flag.

4. **Display**:
   - Implement a function to display the current state of the grid in the console or terminal.
   - Cells that are not yet uncovered should be displayed as a question mark (`?`).
   - Flagged cells should be displayed with a flag symbol (e.g., `F`).

5. **Testing**:
   - Test your game thoroughly to ensure it works as expected and is free of bugs.
   
#### Tips:
- Start with a smaller grid for easier testing and debugging.
- Use a 2D array to represent the grid.
- Use nested loops to initialize the grid and calculate the numbers in each cell.
- Be careful with the grid boundaries to avoid index out of range errors.

#### Bonus:
- A timer to track how long it takes the user to win the game.
- A counter to track the number of moves made by the user.
- Use COLORS
