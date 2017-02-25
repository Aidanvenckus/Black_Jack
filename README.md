# Black_Jack
Black_Jack Python

print("Lets play Black Jack")
import random
card = random.randint(1, 10)
card2 = random.randint(1, 10)
card3 = random.randint(1, 10)
D_card = random.randint(1, 10)
D_card2 = random.randint(1, 10)
D_card3 = random.randint(1, 10)
D_total = D_card + D_card2
total = card + card2
if D_total < 14:
    D_total = D_total + D_card3
print("Card 1:")
print (card)
print("Card 2:")
print (card2)
choice = int(input('Want another card press 1 for yes or anything else for no \n'))
if choice == 1:
    total = total + card3
    print("Card 3:")
    print(card3)
    print("Player Total:")
    print(total)
    print("Dealer Total:")
    print(D_total)
    if total >= 21:
        print("BUST")
    elif total == 21:
        print("Win")
    elif total > D_total:
        print("Win")
    else:
        print("You lose")
else:
    print("Player Total:")
    print(total)
    print("Dealer Total:")
    print(D_total)
    if total >= 21:
        print("BUST")
    elif total == 21:
        print("Win")
    elif total > D_total:
        print("Win")
    else:
        print("You lose")
