# Ideas

## Table of Contents:

- [Mad Libs](#mad-libs)
- [Pick a Number](#pick-a-number)
- [Tic-Tac-Toe](#tic-tac-toe)
- [Hangman](#hangman)
- [Resources](#resources)

## Mad Libs

Implement the famous game of [Mad Libs].

Ask the player for various words, such as:

  - A noun
  - A verb
  - An adjective
  - A place

Then, display a story with their words subsituted into the appropriate
places. For example:

```
Please enter a noun: bicycle
Please enter a verb: dance
Please enter an adjective: green
Please enter another adjective: curvy
...

Your story:

It was a [green], cold November day. I woke up to the [curvy] smell of a
[bicycle] roasting in the oven. Then, I saw my brother [dance] down the
stairs...
```

### Concepts

  - User (keyboard) input
  - Text output
  - String concatenation

### Bonus Ideas

  - Respond with a message if the player doesn't type in a word and make them try
    again.
  - Randomly choose from several stories when the program starts so it's not the
    same every time.


## Pick a Number


### Description

The program should pick a random number between 1 and 100. It should then ask
the player to guess a number. It tells the player whether the number is too high,
too low, or correct. This repeats until the player guesses the right number.

### Concepts

  - If statements
  - While loops
  - User (keyboard) input
  - Parsing (string → number)

### Bonus Ideas

  - Add a number of lives and display a game over message if the player runs out
    of lives.
  - Give a message if the player types in something other than a valid number.

## Tic-Tac-Toe

### Description

Two players can play tic-tac-toe. They can select which squares to play on by
entering the index, 1-9, of a grid like this:

```
1|2|3
-+-+-
4|5|6
-+-+-
7|8|9
```

Every turn alternates between the players, "X" and "O". When a player gets three
in a row, it displays which player won. If all nine squares are filled and no
player won, then a "tie game" message is displayed.

### Concepts

  - 2-dimensional grids/arrays
  - While loops
  - Algorithms (determine if a player has won the game or not)
  - User (keyboard) input
  - Parsing (string → number)

### Bonus Ideas

  - Give a message if the player types in something other than a valid number 1-9.
  - Implement a computer player to play against the human
    - This can be something as simple as choosing a random square that the
      player hasn't chosen yet.

## Hangman

### Description

The program chooses a random word from a set of possible words. It tells the
player how many letters there are and how many lives the player has. It allows
the player to guess one letter at a time.

If the player correctly guesses one of the characters in the word, then every
appearance of that character in the word is shown. If the player correctly
guesses a letter that does not appear in the word, then a life is lost.

After each guess, a partial solution and the number of lives is displayed.

The partial word is displayed where every guessed character is shown and every
unguessed character is replaced by a blank ("`_`"). For example, if the word is
`"apple"`, and the player has guessed `'a'`, `'e'`, and `'l'`, then the word
would appear as:

```
a__le
```

This is repeated until either the player guess all the characters in the word or
until the player runs out of lives.

### Concepts

  - While loops
  - If statements
  - Random choices
  - User (keyboard) input
  - Algorithms (does the guess appear in the word, displaying correct partial
    word)

### Bonus Ideas

Display a text drawing of a hangman instead of just the number of lives. One
part of the man is drawn for every wrong guess. A full hangman may look like
this:

```
   ____
  |    |
  |    o
  |   /|\
  |    |
  |   / \
 _|_
|   |______
|          |
|__________|
```

# Resources

  - [codecademy](https://www.codecademy.com/courses/learn-java/)
    - Step-by-step tutorials.
    - Instructions, editor, and output all in one screen.
  - Google
    - ["How do I get a random number in Java?"](https://www.google.com/search?q=How+do+I+get+a+random+number+in+Java)


[Mad Libs]: http://www.madlibs.com/
