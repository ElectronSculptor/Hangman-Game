
# Hangman Game

This repository contains a simple implementation of the classic Hangman game in Python. The game randomly selects a word from a list, and the player has a limited number of guesses to identify the word by guessing individual letters.

## Features

- Loads a list of valid words from a file (`words.txt`).
- Implements key game logic, such as checking if the word has been guessed and tracking available letters.
- Provides immediate feedback after each guess and displays the partially guessed word.
- Limits the number of incorrect guesses to 8.
- Ends the game when the player either correctly guesses the word or runs out of attempts.

## How to Play

1. The computer selects a random word, and you need to guess the word by suggesting letters one at a time.
2. After each guess, you'll be told if the letter is part of the word.
3. The word is displayed with underscores for the remaining unguessed letters.
4. You have 8 guesses before the game is over, so choose wisely!
5. If you guess the word before running out of guesses, you win the game!

## Code Breakdown

### Main Functions:
- `loadWords()`: Loads a list of words from the `words.txt` file.
- `chooseWord(wordlist)`: Selects a random word from the list.
- `isWordGuessed(secretWord, lettersGuessed)`: Checks if all letters of the secret word have been guessed.
- `getGuessedWord(secretWord, lettersGuessed)`: Displays the current state of the guessed word with underscores.
- `getAvailableLetters(lettersGuessed)`: Displays the remaining letters that haven't been guessed yet.
- `hangman(secretWord)`: Main function that handles the game loop, including managing guesses and feedback.

## Running the Game

1. Make sure you have a `words.txt` file in the same directory as the script.
2. Uncomment the following lines at the bottom of the script to start the game:

\`\`\`python
secretWord = chooseWord(wordlist).lower()
hangman(secretWord)
\`\`\`

3. Run the script:

\`\`\`bash
python hangman_game.py
\`\`\`

4. Follow the prompts in the terminal to guess the word.

## Requirements

- Python 3.x
- A `words.txt` file containing a list of words.

## License

This project is open source and available under the MIT License.
