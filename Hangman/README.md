## Hangman Game Algorithm

### Initialization:
- Import necessary libraries (`stdio.h`, `stdlib.h`, `string.h`, `ctype.h`, `time.h`).
- Declare function prototypes for `drawHangman` and `strlwr`.
- Define `main` function:
  - Declare variables and arrays for the game:
    - `choice` for user input to play again.
    - `guessWords` array containing words for the game.
    - `randomIndex` to randomly select a word index.
    - `numLives` for tracking remaining lives.
    - `numCorrect` for counting correct guesses.
    - `oldCorrect` to compare with `numCorrect` for wrong guesses.
    - `lengthOfWord` for the length of the selected word.
    - `letterGuessed` array to track guessed letters.
    - `quit` to determine if the user quit early.
    - `loopIndex` for iterating over the word.
    - `reguessed` to check if a letter has been guessed before.
    - `guess` array to store user input.
    - `letterEntered` to store the guessed letter.

### Game Loop:
- Start a do-while loop to allow multiple game plays.
  - Seed the random number generator with `srand(time(NULL))`.
  - Randomly select a word index (`randomIndex`) from `guessWords`.
  - Initialize game variables (`numLives`, `numCorrect`, `oldCorrect`, etc.).
  - Start a while loop for each turn of the game until the word is guessed or lives run out.
    - Display the current state of the word with underscores for unguessed letters.
    - Display the hangman figure based on the number of incorrect guesses.
    - Prompt the player for a letter guess.
    - Convert the guess to lowercase using the `strlwr` function.
    - Check if the player wants to quit (`strncmp(guess, "quit", 4)`).
    - Clear the console screen (`system("clear")` or `system("cls")`).
    - Process the user's guess:
      - Check if the letter has already been guessed.
      - Update the game state based on the guess.
    - Check if the player has won or lost.
      - If the player wants to quit, exit the loop.
  - Display the game result (win, lose, or quit).
  - Ask the player if they want to play again (`printf("\nDo you want to Play Again?(Y/N)\n")`).
  - Read the player's choice into the `choice` variable.
- Continue the loop if the player wants to play again (`while (choice == 'Y' || choice == 'y')`).

### Drawing the Hangman:
- Implement the `drawHangman` function to display the hangman figure based on the number of lives.

### Convert String to Lowercase:
- Implement the `strlwr` function to convert a string to lowercase.

### End of Program:
- Return 0 from the `main` function.

