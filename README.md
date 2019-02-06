# 📖 Constructor-Word-Guess-Game

## Overview
This is a Word Guess game built with constructor functions. It is a **command line node app** that takes in parameters and gives you back data. The game receive user input using the `inquirer`, `chalk`, `figlet` and `boxen` npm packages.
####   :point_right: Click  **[>>>Here<<<](https://youtu.be/ZH--1385PGc)**  Check my :tv: video to see how it works.
![concert](/imgs/w7.jpg)


## 📓 Instruction
```
When start, game will pick a Incredible movie character name word. 
The player has 6 chances to find out the name by enter any letter.
System will let you know if your choices are right or wrong. 
If right, your letter will display in the word on the screen.
If you find out the word by the 6 chances you win. 
If wrong, you will lose 1 chance until game over. Thank you for playing.
```
                    
##  ✒️ 1. **Letter.js**: 
Contains a constructor, Letter. This constructor is able to either display an underlying character or a blank placeholder (such as an underscore), depending on whether or not the user has guessed the letter. That means the constructor should define:

  * A string value to store the underlying character for the letter
  * A boolean value that stores whether that letter has been guessed yet
  * A function that returns the underlying character if the letter has been guessed, or a placeholder (like an underscore) if the letter has not been guessed
  * A function that takes a character as an argument and checks it against the underlying character, updating the stored boolean value to true if it was guessed correctly

 
![concert](/imgs/scr5.png)


## ✒️ 2. **Word.js**: 
Contains a constructor, Word that depends on the Letter constructor. This is used to create an object representing the current word the user is attempting to guess. That means the constructor should define:

  * An array of `new` Letter objects representing the letters of the underlying word
  * A function that returns a string representing the word. This should call the function on each letter object (the first function defined in `Letter.js`) that displays the character or an underscore and concatenate those together.
  * A function that takes a character as an argument and calls the guess function on each letter object (the second function defined in `Letter.js`)

![concert](/imgs/scr6.png)


## ✒️ 3.  **index.js**: 

The file containing the logic for the course of the game, which depends on `Word.js` and:

  * Randomly selects a word and uses the `Word` constructor to store it
  * Prompts the user for each guess and keeps track of the user's remaining guesses

![concert](/imgs/scr7.png)


## Author
* [Isaac Wu](https://github.com/squall2046)
* [Game Repo](https://github.com/squall2046/Constructor-Word-Guess)

## Copyright
Isaac Wu © 2019 All Rights Reserved

