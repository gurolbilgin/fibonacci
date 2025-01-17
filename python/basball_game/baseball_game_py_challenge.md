<br>

**Important Note:** *This is a python interview coding challenge, needs to be solved in 20 minutes. You will face those kinds of challenges in most of the interview processes.*

<br>
<br>
<br>

<p align="center"><b>BASEBALL GAME</b></p>

<br>

You are keeping score for a baseball game with strange rules. The game consist of several rounds, where the scores of past rounds may affect future rounds' scores.

At the beginning of the game, you start with an empty record. You are given a list of strings ```ops```, where ```ops[i]``` is the ith operation you must apply to the record and is one of the following:
- **An integer x** - Record a new score of x,
- **"+"** - Record a new score that is the sum of the previous scores. It is guaranteed there will always be two previous scores.
- **"D"** - Record a new score that is double the previous score. It is guaranteed there will always be a previous score.
- **"C"** - Invalidate the pevious score, removing it from the record. It is guaranteed there will always be a previous score.

*Return the sum of all the scores on the record.*

<br>
<br>

**Example 1:**
```
Input: ops = ["5", "2", "C", "D", "+"]
Output: 30
```
*Explanation:*
- "5" - Add 5 to the record, record is now [5],
- "2" - Add 2 to the record, record is now [5, 2],
- "C" - Invalidate and remove the previous score, record is now [5],
- "D" - Add 2 * 5 = 10 to the record, record is now [5, 10],
- "+" - Add 5 + 10 = 15 to the record, record is now [5, 10, 15],

*The total sum is 5 + 10 + 15 = 30.*

<br>
<br>
<br>

**Example 2:**
```
Input: ops = ["5", "-2", "4", "C", "D", "9", "+", "+"]
Output: 27
```

*Explanation:*

- "5" - Add 5 to the record, record is now [5],
- "-2" - Add -2 to the record, record is now [5, -2],
- "4" - Add 4 to the record, record is now [5, -2, 4],
- "C" - Invalidate and remove the previous score, record is now [5, -2],
- "D" - Add 2 * -2 = -4 to the record, record is now [5, -2, -4],
- "9" - Add 9 to the record, record is now [5, -2, -4, 9],
- "+" - Add -4 + 9 = 5 to the record, record is now [5, -2, -4, 9, 5],
- "+" - Add 9 + 5 = 14 to the record, record is now [5, -2, -4, 9, 5, 14],

*The total sum is 5 + -2 + -4 + 9 + 5 + 14 = 27.*

<br>
<br>

Please don't hesitate to ask any questions with a thread under this message!

Please share your solutions using direct mesage on slack to _@Rafe Stefano_


**_Happy coding!_** 😃