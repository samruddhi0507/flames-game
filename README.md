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

```
FLAMES
counting is start from F, E is at 5th count so we remove E and start counting again but a this time start from S.
FLAMS
M is at 5th count so we remove M and counting start from S.
FLAS
S is at 5th count so we remove S and counting start from F.
FLA
L is at 5th count so we remove L and counting start from A.
FA
A is at 5th count so we remove A. now we have only one letter is remaining so this is the final answer.
F
So, the relationship is F i.e. Friends .

```
### Approach: 

Take two names as input then remove the common characters with their respective common occurrences. For removing purpose we create user-defined remove_match_char function with two arguments as list1 and list2 which stores list of characters of two players name respectively and return list of concatenated list(list1 + “*” flagst2) and flag value which we store in ret_list variable.After removing all the common characters, count the total no. of remaining characters then create a result list with FLAMES acronym i.e [“Friends”, “Love”, “Affection”, “Marriage”, “Enemy”, “Siblings”]. Now start removing word one by one untill list not contains only one word, using the total count which we got. the word which remains in the last, is the result.











