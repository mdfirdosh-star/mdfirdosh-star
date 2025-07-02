# pizza program
pizza_size=(input("enter your pizza size \n m,s,l").lower())
cold_drink=(input("should you want to cold drink \n y, n")).lower()
total_bill=0
if pizza_size=="s":
    total_bill+=200
elif pizza_size=="m":
    total_bill+=250
elif pizza_size=="l":
    total_bill+=300
else:
    print("valid pizza size ")
if cold_drink=="y":
    total_bill+=60
else:
    pass
print(total_bill)




# Roller Coaster project
hight =int(input("enter your hight in cm  "))
if hight>=120:
    print("i can enter the rollar coaster ")
    age=int(input("enter your age"))
    if age>=18:
        print("rs 120")
    elif 1<age and age<7:
        print("rs 30 and with gargain")
    else:
        print()

else:
    print("enter your valid hight")




# project game 
print("welcome to my game ")
print("chose the correct option and win the game")
value=input("chose the option \n left, right\n")
if value=="left":
    print("you can pass the game and convert the second round ")
    print()
    value2=input("chose the option \n up, down\n")
    if value2=="down":
        print("you chose the correct option and convert the third round ")
        print()
        value3=input("chose the option \n good, bad\n")
        if value3=="good":
            print("you win the game")
            print()
        else:
            print("game over")
    else:
        print("game over")
else:
    print("game over")


# pasword generator poject
import random 
chr= ['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 
                     'i', 'j', 'k', 'm', 'n', 'o', 'p', 'q',
                     'r', 's', 't', 'u', 'v', 'w', 'x', 'y',
                     'z','A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 
                     'I', 'J', 'K', 'M', 'N', 'O', 'P', 'Q',
                     'R', 'S', 'T', 'U', 'V', 'W', 'X', 'Y',
                     'Z']
s = ['@', '#', '$', '%', '=', ':', '?', '.', '/', '|', '~', '>', 
           '*', '(', ')', '<']
d = ['0', '1', '2', '3', '4', '5', '6', '7', '8', '9'] 
pasword=""
chr_1=int(input("how many char in use to password"))
s_1=int(input("how many symbol in use to password"))
d_1=int(input("how many degit in use to password"))
for i in range(0,chr_1):
    pasword+=random.choice(chr)
for i in  range(0,s_1):
    pasword+=random.choice(s)
for i in range(0,d_1):
    pasword+=random.choice(d)
print(pasword)



# day1
# hangman project
import random 
word=["happy","singh","mohan","sohan"]
choise=random.choice(word)
print(choise)
guss=input("enter your value \n" ).lower()
print(guss)
for i in choise:
    if i==guss:
        print("right")
    else:
        print("wrong")


# day2
# project of random value chose in the list and the value all word show the blank space

import random 
list1=["firdosh","shaiyad ","izaril","apple"]
choice=random.choice(list1)
print(choice)
placeholder=" "
word_length=len(choice)
for positiion in range(word_length):
    placeholder+="-"
print(placeholder)
guss=input("enter your value \n" ).lower()
print(guss)

display=""
for i in choice:
    if i==guss:
        display+=i
    else:
        display+="-"
print(display)







# project of hangman 
import random
list=["firdosh","mohan","sohan","himayu"]
random_choice=random.choice(list)
print(random_choice)

placeholder=""
length=len(random_choice)
for position in range(length):
    placeholder+="-"
print(placeholder)


game_over=False
correct_letter=[]
while not game_over:
    guss=input("enter your word \n ").lower()
    display=""
    for i in random_choice:
        if i==guss:
            display+=i
            correct_letter.append(guss)
        elif i in correct_letter:
            display+=i
        else:
            display+="_"
    print(display)



    # projecr step 4

lavel=[''' _______
     |/      |
     |      (_)
     |      \|/
     |       |
     |      / \
     |
 jgs_|___ ''','''
    _______
     |/      |
     |      (_)
     |      \|/
     |       |
     |      / 
     |
 jgs_|___
''',''' _______
     |/      |
     |      (_)
     |      \|/
     |       |
     |      
     |
 jgs_|___''',''' _______
     |/      |
     |      (_)
     |      \|/
     |       
     |
     |
 jgs_|___''',''' _______
     |/      |
     |      (_)
     |      \|
     |       
     |      
     |
 jgs_|___''','''  _______
     |/      |
     |      (_)
     |      \
     |       
     | 
     |
 jgs_|___''','''  _______
     |/      |
     |      (_)
     |      
     |      
     |   
     |
 jgs_|___''']


import random
list=["firdosh","mohan","sohan","himayu"]


part=7
random_choice=random.choice(list)
print(random_choice)

placeholder=""
length=len(random_choice)
for position in range(length):
    placeholder+="-"
print(placeholder)


game_over=False
correct_letter=[]
while not game_over:
    guss=input("enter your word \n ").lower()
    display=""
    for i in random_choice:
        if i==guss:
            display+=i
            correct_letter.append(guss)
        elif i in correct_letter:
            display+=i
        else:
            display+="_"
    print(display)

   
    if guss not in random_choice:
        part-=1
        if part==0:
            game_over=True
            print("you lose the game")

    if "-" not in display:
        game_over=True
        print("win the game")
    print(lavel[part])

