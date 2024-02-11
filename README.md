# Memory-Card-Game
A simple memory card game built with HTML, CSS, and JavaScript.


Introduction:
This is a classic memory card game where the player needs to match pairs of cards with the same image. The game is implemented using HTML for structure,
CSS for styling, and JavaScript for functionality.

How to Play:
1.Click on a card to flip it and reveal the image.
2.Click on a second card to try and match it with the first one.
3.If the cards match, they stay flipped. If not, they flip back.
4.Match all the pairs to win the game.
5.You have 6 lives to complete the game.

Functions:
1.getData() :
-Generates an array of objects containing image sources and names for the cards.
-Return Value--> An array of card data objects.

2.randomize() :
-Shuffles the card data array to create a random order for the cards.
-Return Value--> The shuffled card data array.

3.cardGenerator() :
-Generates HTML for the game cards and attaches event listeners.
-Called during the initialization of the game.

4.checkCards(e) :
-Checks if the flipped cards match and updates the game state accordingly.
-Parameters-->
  - "e" (Event)--> The click event object.
- *Logic*
  - If two flipped cards match, they stay flipped.
  - If not, the cards flip back, and the player loses a life.
  - Updates the player's lives and checks if the game is won or lost.

5.restart(text) :
-Restarts the game with a new set of cards and updates the player's lives.
-Parameters-->
  - "text" (String): The message to be displayed.
- *Logic*
  - Resets card data, flips cards back, and randomizes their positions.
  - Updates player lives and displays a message.
  - Shows cards for 1 second after resetting.
