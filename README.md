# flames-game

Let’s create a simple FLAMES game without using any external game libraries like PyGame.

FLAMES is a popular game named after the acronym: Friends, Lovers, Affectionate, Marriage, Enemies, Sibling. This game does not accurately predict whether or not an individual is right for you, but it can be fun to play this with your friends.

There are two steps in this game:

### Get the count :

 * Take the two names.
* Remove the common characters with their respective common occurrences.
* Get the count of the characters that are left .

### Get the result :


* Take FLAMES letters as [“F”, “L”, “A”, “M”, “E”, “S”]
* Start removing letter using the count we got.
* The letter which last the process is the result.

### Example :
```
Input :   player1 name : AJAY
          player 2 name : PRIYA

Output : Relationship status : Friends

```
### Explanation: 

In above given two names A and Y are common letters which are occurring one time(common count) in both names so we are removing these letters from both names. Now count the total letters that are left here it is 5. Now start removing letters one by one from FLAMES using the count we got and the letter which lasts the process is the result.
Counting is done in anti-clockwise circular fashion.
