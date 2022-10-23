# Dice-Simulator
#### Subject taught by the teacher Rodrigo Lyra

### Confirming Odds

We see a lot of probabilities in everyday life, but are they correct? With the use of algorithms we can clean it up, do tests and check what is happening. We roll a six-sided die 10 times and the number 5 lands 5 times, is the die biased? are the odds wrong? We can roll the dice 10,000 times and get the real proof, in the real world this is unlikely, but in algorithms...

We can generate random integers with the rand() function, which combined with the % operator, generates an integer value between 0 and NUMBER, not including the NUMBER:
#### rand() % <NUMBER>
  
To use this function without returning the same numbers every run, we need at the beginning of the program, and only once, to arrange the seed for generating the numbers at the same time, for this we also need to include the <time.h> library:
#### #include <time.h>
#### srand(time(NULL));
  
So let's do the following, first a function that asks the user to choose between 3 options: 1. Roll a die 2. Roll more than one die 3. Evaluate Monty Hall's problem (CHALLENGE)
  
If the option to roll a die is chosen, another reading function must be called , this will read the number of sides of the die (between 1 and 100) and the number of roll repetitions (greater than 0).
  
After reading there will be a function that receives as parameter the number of sides in the die and the number of rolls, make the number of rolls passed by parameter with a die with that number of sides (use the rand() function). Each result must be added into a vector that will serve as a counter.
  
Then a function must be called that receives this counter vector per parameter and the number of rolls and writes on the screen each value and the percentage of times it has fallen (count of each position / number of rolls).
  
If the option to roll more than one dice is chosen, another reading function must be called , this will read the number of dice and the number of sides of the dice (the total possible sum of result must be less than 100, for example, 3 20-sided dice add up to a maximum of 60, so it can, 15 10-sided dice add up to a maximum of 150, so it cannot) and the number of repeat rolls (greater than 0).
  
After reading, there will be a function that receives by parameter the number of dice and sides in the dice and the number of rolls, make the number of rolls passed by parameter with that amount of dice and sides (use the rand() function). Each sum of data results must be added in a vector that will serve as a counter.
  
Then a function must be called that receives this counter vector per parameter and the number of rolls and writes on the screen each value and the percentage of times it has fallen (count of each position / number of rolls).

(CHALLENGE) Prove the Monty Hall problem, do a simulation of thousands of games with 3 doors and prove the change of choice increases the probability of winning to 66%. More information about the issue at https://en.wikipedia.org/wiki/Problema_de_Monty_Hall 

- Options reading functions must be passed as variables to be read byparameter (by reference);

- To save the statistical data, make a vector of 100 positions and use up to the value that is needed, make a function that resets all its values
paragraph 0;

- The display function as statistics must be one, called by the rotation functions
one die or more than 1;

- Both the function of rolling one or more dice must have the same name, they must be
of;

- The Monty Hall problem is a challenge, it has no weight in the paper's grade, I will give
extra points for creative solutions.
