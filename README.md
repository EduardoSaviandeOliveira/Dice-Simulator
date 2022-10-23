# Dice-Simulator

### Confirming Odds
We see a lot of probabilities in everyday life, but are they correct? with the use of
This can be done to test and verify what we can, we can be sure of.
We roll a six-sided die 10 times and the number 5 lands 5 times, is the die biased? As
Are the odds wrong? We can roll the dice 10,000 times and get the real proof, no
real world that is, but in
We can generate random integers with the rand() function, which are allied to the operator
%, generates an integer value between 0 and NUMBER, not including the NUMBER:
rand() % <NUMBER>
To use this function without returning the same numbers every run,
we don't need to start the program, and only once, fix the seed of generation of the
numbers at the time, for this you must also include a <time.h> library:
#include <hour.h>
srand(time(NULL));
We start by doing the following, a function so let's ask the user
choose from 3 options:
1. Roll a die
2. Roll more than one die
3. Evaluate Monty Hall's Problem (CHALLENGE)
If the option to roll a die is chosen, another reading function must be called,
this will read the number of sides of the die (between 1 and 10) and the number of repetitions0 of
scroll (greater than 0).
After reading there will be a function that receives as parameter the number of sides not
die and the number of rolls, make the number of rolls passed by parameter with
a die with that many sides (use the rand() function). must be added
each result in a vector that will serve as a counter. Then a function must be called that receives this counter vector by parameter
and the number of rolls and write on the screen each value and the percentage of times it fell
(count of each position / number of rolls).
Figure 1. Example of rolls that should happen if the user asks for 12 rolls of
4 sided dice
Figure 2. Example of the vector and the function output for the throws in the previous figure
If the option to roll more than one die is chosen, another function must be called.
read, this will read the number of dice and the number of sides of the dice (the total possible sum
result must be less than 100, e.g. 3 20-sided dice does not produce
max the sum of 60, so can, 15 10-sided dice add up to 150 max, so
can) and the number of non-scroll repetitions (greater than 0).
After reading, there will be a function that receives as a parameter the number of data and
sides on the dice and the number of rolls, make the number of rolls passed by
Parameter with the amount of data and sides (use the rand() function). should
be added sum of results of the data in a vector that will serve as
counter. Then a function must be called that receives this counter vector by parameter
and the number of rolls and write on the screen each value and the percentage of times it fell
(count of each position / number of rolls).
Figure 3. Example of rolls if the input for 3 rolls of 5 8-sided dice.
Figure 4. Example of part of the output for the above results, remembering that the output of
program must be complete.
(CHALLENGE) Prove the Monty Hall problem, do a simulation of thousands of
games with 3 doors and prove the change of choice increases the probability of winning
to 66%. More information about the issue at
https://en.wikipedia.org/wiki/Problema_de_Monty_Hall 

- Options reading functions must be passed as variables to be read byparameter (by reference);

- To save the statistical data, make a vector of 100 positions and use;

up to the value that is needed, make a function that resets all its values
paragraph 0;

- The display function as statistics must be one, called by the rotation functions
one die or more than 1;

- Both the function of rolling one or more dice must have the same name, they must be
of;

- The Monty Hall problem is a challenge, it has no weight in the paper's grade, I will give
extra points for creative solutions.
