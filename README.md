# python-first-code
#first project guess number game

import random

jackpot = random.randint(1, 100)
guess = int(input('Guess any number between 1 and 100: '))
counter = 1

while guess != jackpot:
    if guess < jackpot:
        print('Galat! Try a higher number.')
    else:
        print('Galat! Try a lower number.')

    guess = int(input('Guess again: '))
    counter += 1

print('🎉 Guest correct!')
print('Attempts:', counter)

