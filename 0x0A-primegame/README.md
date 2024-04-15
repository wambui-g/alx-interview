For this project, you will need to leverage your understanding of prime numbers, game theory, and algorithm optimization to solve a competitive game scenario. The challenge involves determining the winner of a game based on the strategic removal of prime numbers and their multiples from a set of consecutive integers.

Concepts Needed:
Prime Numbers:

Understanding what prime numbers are.
Efficient algorithms for identifying prime numbers within a range.
Sieve of Eratosthenes:

An efficient algorithm for finding all prime numbers up to any given limit, which can be particularly useful for this task.
Game Theory:

Basic principles of competitive games where players take turns and the concept of optimal play.
Understanding win conditions and strategies that lead to a win or loss.
Dynamic Programming/Memoization:

Using previous results to make future calculations faster, potentially necessary for optimizing the solution for multiple rounds of the game.
Python Programming:

Loops and conditional statements for implementing game logic and algorithms.
Arrays and lists for storing the integers and tracking removed numbers.

Resources:
https://www.geeksforgeeks.org/sieve-of-eratosthenes/
https://www.investopedia.com/terms/g/gametheory.asp
https://skerritt.blog/dynamic-programming/
https://docs.python.org/3/tutorial/introduction.html#lists

Task
Maria and Ben are playing a game. Given a set of consecutive integers starting from 1 up to and including n, they take turns choosing a prime number from the set and removing that number and its multiples from the set. The player that cannot make a move loses the game.

They play x rounds of the game, where n may be different for each round. Assuming Maria always goes first and both players play optimally, determine who the winner of each game is.

Prototype: def isWinner(x, nums)
where x is the number of rounds and nums is an array of n
Return: name of the player that won the most rounds
If the winner cannot be determined, return None
You can assume n and x will not be larger than 10000
You cannot import any packages in this task
Example:

x = 3, nums = [4, 5, 1]
First round: 4

Maria picks 2 and removes 2, 4, leaving 1, 3
Ben picks 3 and removes 3, leaving 1
Ben wins because there are no prime numbers left for Maria to choose
Second round: 5

Maria picks 2 and removes 2, 4, leaving 1, 3, 5
Ben picks 3 and removes 3, leaving 1, 5
Maria picks 5 and removes 5, leaving 1
Maria wins because there are no prime numbers left for Ben to choose
Third round: 1

Ben wins because there are no prime numbers for Maria to choose
Result: Ben has the most wins
