# Hangman-Game

Game Description:

- This is a classic hangman word guessing game where the player tries to guess a random secret word before they run out of attempts. As wrong guesses are made, more of the visual "hangman" figure is drawn.

Game Rules:

- The game randomly selects a secret word 
  from the word list
- The player starts with 8 incorrect 
  guess attempts
- Each round the player guesses 1 letter
  Correct letters are revealed in the secret word
- Incorrect letters add to the  "hangman" visual
- The player wins if they revealed the 
  full word before 8 incorrect attempts
- The player loses if the hangman figure 
  is fully drawn before solving the word

Code Overview:

- HANGMAN_PICS: List of ascii art for 
  hangman stages
- WORDS: List of possible words to pick 
  from
- main(): Runs game loop, calls other 
  functions
- draw_hangman(): Prints hangman visual 
  based on wrong guesses
- random_word(): Picks random word for 
  game
- get_valid_guess(): Gets and validates 
  player's letter guess
- update_revealed_letters(): Reveals 
  matching letters
- display_win()/display_loss(): Print end 
  game messages

Expanding the Game:

- Add difficulty levels with different 
  word lists
- Allow player to choose/enter category   for words
- Add ability to save and display player 
  statistics
- Support multiplayer via local hot seat 
  or networked
- Improve graphics with images instead of 
  ascii art
- Add ability to guess full word instead 
  of just letters
- Implement hint system to reveal random letter
- Add list of previously guessed letters
- Add variety with categories (fruits, 
  animals etc)
- Incrementally increase size of word list
- Track number of wins and losses
- Allow player to play again without 
  restart

Game Instructions:
  - The computer will pick a random secret word. Try guessing one letter at a time. If a letter is in the word, it will get revealed. If not, the hangman image will get filled in more. Keep guessing until you solve the word or until the stickman image is fully drawn to lose. Good luck!

Game Report:
  - This hangman game implementation utilizes modular programming by separating the logical pieces of code into individual functions like main(), draw_hangman(), get_valid_guess(), etc. This makes the code more organized and maintainable. The main() function handles controlling overall game state and flow. Key functionality is abstracted into the additional modular functions it calls. For example, random_word() selects a secret word randomly each game to allow for replayability, while get_valid_guess() handles getting user input and validating the guess which improves user experience.

  - The display functions like draw_hangman() and printing the revealed word slots provide visual feedback to the player each round to keep them engaged. As incorrect guesses build up, more of the ascii art hangman graphic is revealed and body parts filled in. This combined with the revealed letters from correct guesses gives the user a progress update on the current game state.

  - The modular organization and game flow with validation, input/output feedback, and randomization come together to create an enjoyable command line hangman game implementation. Opportunities to expand the game could include upgrading the graphical elements, adding difficulty options, or enabling multiplayer support. Overall it utilizes common programming techniques well to build a fully functional small game from scratch.