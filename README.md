# snake-water-gun-using-python
It is the most popular game of snake, water gun that i have created using basic python functions! do try to play and review it!

HERE IS THE CODE!


# Snake Water Gun
import random
print('WELCOME TO THE GAME OF SNAKE,WATER GUN!')
user = 0
computer = 0
i = 0
while i < 10:
    print('Enter your choice snake, water and gun : ')
    lst = ['snake', 'water', 'gun']
    user_input = input()
    computer_input = random.choice(lst)
    if user_input == 'snake':
        lst1 = ['gun', 'water']
        computer_input = random.choice(lst1)
        if computer_input == 'gun':
            print('Computer won!')
            computer = computer+1
        elif computer_input == 'water':
            print('User won!')
            user = user+1
        else:
            print('It"s a tie! No points!')
    elif user_input == 'water':
        lst2 = ['snake','gun']
        computer_input = random.choice(lst2)
        if computer_input == 'snake':
            print('Computer won!')
            computer = computer+1
        elif computer_input == 'gun':
            print('User won!')
            user = user+1
        else:
            print('It"s a tie! No points!')
    elif user_input == 'gun':
        lst2 = ['water','gun']
        computer_input = random.choice(lst2)
        if computer_input == 'water':
            print('Computer won!')
            computer = computer+1
        elif computer_input == 'gun':
            print('User won!')
            user = user+1
        else:
            print('It"s a tie! No points!')
    i = i+1
    print(10-i,'chances are left!')


if user>computer:
    print('Hurray! User wins')
elif user<computer:
    print('Computer wins! Better luck next time!🥺')
else:
    print('It"s a Tie! Try Again!')
