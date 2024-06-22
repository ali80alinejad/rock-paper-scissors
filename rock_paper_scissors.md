# how make rock paper scissors

## step 1
we should import random module for random rock or paper or scissors
```python 
import random
```
## step 2
Create a variable for how do you want to play
```python 
set_game=int(input('how many rounds do you want play? '))
```
## step 3
make while loop for how many time play game
```python
while set_game>0:
```
## step 4
Betting and scoring
```python
your_choice=input('enter your choice: ')
    game=['rock','paper','scissors']
    computer=random.choice(game)
    computer_point=0
    you_point=0
    if your_choice=='rock'and computer=='scissors':
        you_point+=1
    if your_choice=='rock'and computer=='paper':
        computer_point+=1
    if your_choice=='paper'and computer=='rock':
        you_point+=1
    if your_choice=='paper'and computer=='scissors':
        computer_point+=1
    if your_choice=='scissors'and computer=='rock':
        computer_point+=1
    if your_choice=='scissors'and computer=='paper':
        you_point+=1 
```
## step 5
Show points and choices
```python
    print('you(',your_choice,')',  you_point,    'com(',computer,')', computer_point)
    set_game-=1
if you_point>computer_point:
    print('you win')
if computer_point>you_point:
    print('you lose')
```