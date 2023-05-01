Download Link: https://assignmentchef.com/product/solved-bbm103-assignment-2-hangman
<br>
<strong>In And Out </strong>is a game somewhat similar to Hangman, but with a very interesting twist. At the beginning of the game, a hidden word is chosen. The play starts with the <strong>IN </strong>mode. The player guesses a letter. If the player guesses correctly, the letter is revealed in the hidden word and he / she can guess another letter that has not been used in the <em>IN </em>mode before. The game continues like this until the player guesses a letter which is not in the word or the letter which has been guessed before in the <em>IN </em>mode. At this point, the play turns into the <strong>OUT </strong>mode and the player is required to guess a letter which he / she thinks is <em>NOT </em>in the word and has not been used in <em>OUT </em>mode before. If the player is incorrect, the mode stays in the <strong>OUT </strong>mode, and he / she loses points each time he / she guesses incorrectly. Once the player guesses a letter which is not in the word and has not been guessed in the <em>OUT </em>mode before, the play turns into the <strong>IN </strong>mode again, and the player can resume guessing letters he / she thinks are in the word.

The player has 5 guess chances to guess the word incorrectly or guess the already used letters in modes. If the player finds the word before 5 chances are used, he / she becomes the winner. But if the player can’t find the word before making 5 incorrect guesses, he / she becomes the loser.

1

<h1>ASSIGNMENT</h1>

Your assignment is to write a computer program which plays a game of <strong>IN AND OUT</strong>. In particular, your program should do the following:

<ol>

 <li>Set the word which is taken as an argument from the command line.</li>

 <li>Set the letter list taken as an argument from the command line.</li>

 <li>Play a game of <em>IN AND OUT </em>using the algorithm, as described below:

  <ul>

   <li>Print out how many guess chances the user has remaining.</li>

   <li>Take a letter from the letter list. If player is in the <strong>IN </strong>mode and the picked letter is in the word and the letter has not been used in the <em>IN </em>mode before, reveal the corresponding hidden letter or letters in the word. Repeat this step until the picked letter is not in the word or the letter has been guessed in the <em>IN </em>mode before.</li>

   <li>If the letter is not in the word or it has been guessed in the <em>IN </em>mode before, and if the player is in the <strong>IN </strong>mode, change the mode into the <strong>OUT </strong>mode and decrease the guess chances.</li>

   <li>If the letter is not in the word and it has not been guessed in the <em>OUT </em>mode before and the player is in the <strong>OUT </strong>mode, change the mode into the <strong>IN </strong> Otherwise, stay in the <strong>OUT </strong>mode and decrease the guess chances.</li>

   <li>When all hidden letters are revealed and the number of remaining guess chances is bigger than 0, print to the screen the following message: ”You won the game”. If there are still remaining letters in the letter list and there aren’t any guess chances left, print to the screen the following message: ”You lost the game” Example 1: python3 assignment2.py car c,e,y,a,m,q,r</li>

  </ul></li>

</ol>

You have 5 guesses left

[’-’, ’-’, ’-’]

——————————————–

Guessed word: c You are in IN mode

You have 5 guesses left

[’c’, ’-’, ’-’]

——————————————-Guessed word: e The game turned into OUT mode

You have 4 guesses left

[’c’, ’-’, ’-’]

——————————————–

Guessed word: y The game turned into IN mode

You have 4 guesses left

[’c’, ’-’, ’-’]

——————————————–

Guessed word: a You are in IN mode

You have 4 guesses left

[’c’, ’a’, ’-’]

——————————————–

Guessed word: m The game turned into OUT mode

You have 3 guesses left

[’c’, ’a’, ’-’]

——————————————–

Guessed word: q The game turned into IN mode

You have 3 guesses left

[’c’, ’a’, ’-’]

——————————————–

Guessed word: r You are in IN mode

You have 3 guesses left

[’c’, ’a’, ’r’]

——————————————-You won the game Example 2: python3 assignment2.py deneme d,e,n,e,y,y,m

You have 5 guesses left

[’-’, ’-’, ’-’, ’-’, ’-’, ’-’]

——————————————–

Guessed word: d You are in IN mode

You have 5 guesses left

[’d’, ’-’, ’-’, ’-’, ’-’, ’-’]

——————————————–

Guessed word: e You are in IN mode

You have 5 guesses left

[’d’, ’e’, ’-’, ’e’, ’-’, ’e’]

——————————————–

Guessed word: n You are in IN mode

You have 5 guesses left

[’d’, ’e’, ’n’, ’e’, ’-’, ’e’]

——————————————–

Guessed word: e is used in IN mode. The game turned into OUT mode

You have 4 guesses left

[’d’, ’e’, ’n’, ’e’, ’-’, ’e’]

——————————————–

Guessed word: y The game turned into IN mode

You have 4 guesses left

[’d’, ’e’, ’n’, ’e’, ’-’, ’e’]

——————————————-Guessed word: y The game turned into OUT mode

You have 3 guesses left

[’d’, ’e’, ’n’, ’e’, ’-’, ’e’]

——————————————–

Guessed word: m You are in OUT mode

You have 2 guesses left

[’d’, ’e’, ’n’, ’e’, ’-’, ’e’]

——————————————–

You finished all letters

You lost the game