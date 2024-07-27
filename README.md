
Hangman Game
This is a text-based version of the classic Hangman game implemented in Python. The game selects a random word from a predefined list and allows users to guess letters. The goal is to guess the entire word before running out of tries.

How to Play
Start the Game: Run the script and the game will start by selecting a random word from a predefined list.
Guess Letters: The user will be prompted to guess a letter.
If the guessed letter is in the word, it will be revealed in its correct positions.
If the guessed letter is not in the word, the user loses a try and part of the hangman is drawn.
Win or Lose:
The user wins if all letters in the word are guessed correctly before running out of tries.
The user loses if they run out of tries before guessing the word. The complete hangman will be displayed, and the correct word will be revealed.
Code Explanation
Functions
choose_word(): Selects a random word from a predefined list.
display_hangman(tries): Returns the current state of the hangman drawing based on the number of incorrect tries.
play_hangman(): The main function that runs the game. It handles the game logic, including:
Initializing the game state.
Prompting the user for guesses.
Updating the display after each guess.
Checking for win/loss conditions.
Game Flow
Initialization:

The game selects a random word.
The word is stored as a set of letters.
An empty set is created to store guessed letters.
The number of tries is set to 6.
User Input:

The user guesses a letter.
The program checks if the guessed letter has been guessed before.
If the guessed letter is in the word, it is added to the set of guessed letters.
If the guessed letter is not in the word, the number of tries is decremented, and the letter is added to the set of guessed letters.
Display Update:

The hangman display is updated based on the number of incorrect tries.
The current state of the word is displayed, showing correctly guessed letters and underscores for remaining letters.
End Game:

The game checks if the user has guessed all the letters in the word (win condition).
The game checks if the user has run out of tries (loss condition).
