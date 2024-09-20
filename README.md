# U.S. Presidents Matching Game Web App

### Project's Purpose

Because I love learning and teaching United States history, I decided it would be fun to create a game where you match the names and faces of U.S. Presidents. This project shows my skills in using JavaScript for front end web development, as well as some basic skills using HTML and CSS styles. I really enjoyed working on this project. It’s quite fun to play, and the end result looks beautiful.

### Game Levels

The game has three levels. Each level has the cards with the names and pictures of six U.S. presidents. Level one includes presidents from George Washington, in 1789, to James Monroe in 1829. Level two goes from Andrew Jackson to Zachary Taylor, and Level three contains prominent presidents since 1861, such as Abraham Lincoln, Franklin Delano Roosevelt and Ronald Reagan.

### Playing the Game

After selecting two cards, the player presses the “check match” button. If the pair of cards is a match, the following actions take place on the screen:

- The score increases by 1 point.
- The message “Correct!” appears in the match results.
- Matched cards can no longer be flipped.
- Matched cards are blurred and have a shadow behind them.
  If the pair of cards is not a match, the match results displays the message “not a match.” Once the last match is found, the “next level” button appears, and the player may click it to go on to the next level. There is also a “re-shuffle” button if the player wishes to shuffle the deck and play that round again. The re-shuffle button can be clicked at anytime during the game.

### Writing the Code

Much of the functionality of this game includes using event listeners and JavaScript functions that add and take away CSS classes to change the look of elements on the screen.

Box element - The HTML page contains a box (a div element) that contains the HTML layout for all of the content on the page, such as buttons, rows of cards and the scoreboard. The cards are actually button elements that are made to look like cards. Each HTML page is linked to its own script.js file that controls the logic. All the pages are linked to the same CSS styles file.

Flipping cards – I wrote the flipCard() function that contains a for loop that assigns each card button an image. It also contains an event listener that adds or removes the “hidden” CSS class each time a card is clicked.

Check Match – I wrote three functions that handle the logic to determine whether a pair of cards is a match, which include the isCorrect(), notCorrect(), and findMatch() functions. A fourth function, showMatch() changes the look of the cards when a match is made. An event listener that contains a function with instructions to execute these functions and what happens when a match is found.

Reshuffle – The reshuffle button takes the player to a new, identically looking page where the cards are assigned to different images, and the game level starts from the beginning, with all the cards face down and the score at zero.

### Ways to Improve the Game

Here are some ideas for making the game better.

- When a pair of cards is not a match, the game could flip the cards back over for you.
- Each level of the game looks like a one page app, but the re-shuffle button actually contains a link to a new page that is copy of the first, only with the deck re-shuffled. I think the game could be slightly improved by incorporating an actual random reshuffle logic within the same page instead of taking the player to a new nearly identical HTML page. This might be accomplished by creating a dictionary with keys assigned to each image, and assign the buttons to the key numbers instead of images. That way, the images could be truly randomly re-assigned to buttons each time the re-shuffle button is pressed.
- For those who might cheat, the game could add logic to prevent players from flipping over more than two cards at a time.
- For those who love learning about the presidents, the game could be expanded to include all of the U.S. presidents, which would require 8 levels, since there have been 46 U.S. presidents.

In conclusion, doing this project helped me to learn more about manipulating HTML elements using JavaScript. I also learned to recognize the faces of even more U.S. presidents.
