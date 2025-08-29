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








# project of fake news generater 
#      ||

# using opretions 
# import random module
# create the list (subject, object,placename)
# use of loop 
# use of f_string
# use of strip  
# use of lower methord
# use of if alse astiment
# use of input function 


# import random modules 
import random 

# create the list 
subjects=["Elon Musk",
         "Bill Gates",
         "Taylor Swift",
         "NASA",
         "Cristiano Ronaldo",
         "Google",
         "Kim Kardashian",
         "Jeff Bezos" ]

objects=["Flying cars"
        "Farmland"
        "Mayor position"
        "Alien city"
        "Chocolate factory"
        "Free houses"
        "Space agency",
        "Smartphones",
        "Underwater cinema",]

places=["New York",
        "Texas",
        "Los Angele",
        "Moon",
        "Paris",
        "Dubai",
        "Florida",
        "Washington",
        "Maldives",  ]
# use of loop

while True :
# use of random choice methord
  subject=random.choice(subjects)
  object=random.choice(objects)
  place=random.choice(places)
  headline=(f"FAKE NEWS : {subject} was {object} in {place}")
  print("\n" + headline)
  user_input=input("\ndo you want to another headline print(yesh,no)").strip().lower()
  if  user_input =="no":
    break
print("\n thank you using the headline generator  project ")












# pasward generator project 

# use of random model
# create the list of alphabate 
# create the list of symbol 
# create the list of number 
# user input function use all loop in int(only number )
# pasword valible 
# use of loop
# use of append function 

# use the random function 
import random
# create a empty varible name pasword 
pasword =" "
# create the loop in alphabet
chr=["a","b","c","d","e","f","g","h","i","j","k","l","m",
    "n","o","p","q","r","s","t","u","v","w","x","y","z","A","B","C","D","E","F","G","H","I","J","K","L","M",
    "N","O","P","Q","R","S","T","U","V","W","X","Y","Z"]

symbol=["!", "@", "#", "$", "%", "^", "&", "*", "(", ")", "-", "_",
    "=", "+", "[", "]", "{", "}", ";", ":", "'", '"', ",", ".",
    "<", ">", "/", "?", "|", "\\", "`", "~"]


number=["0","1","2","3","4","5","6","7","8","9"]


# use of input function 

chr_input=int(input("\n how many character is use of pasword ")) 
symbol_input=int(input("\n how many symbol is use of pasword "))
number_input=int(input("\n how many number is use of pasword "))
# use of loop

# create the for loop of for chr 
for i in range(0,chr_input):
  pasword+=random.choice(chr) # add the chr value in pasword

# create the for loop of for sumbol
for j in range (0,symbol_input):
  pasword+=random.choice(symbol) # add the symbol value in pasword

# create the for loop of for number 
for k in range (0,number_input):
  pasword+=random.choice(number) # add the number value in pasword

# use the f_string and print the generate the pasword 
print(f"GENERATED_PASWORD: {pasword} ")









# water snake and gun project
# import random modules 
# import ramdon.randint function
# if ,elif,else conditions
# use return keyword
# input function 
# def function 
# 0=water
# 1=snake
# 2=gun

gun=(""" ⠀⠀⠀⠀⠀⠀⢀⣠⣴⣶⣶⣤⣤⣤⣤⣶⣶⣶⣶⣶⣶⣦⣤⣤⡀⠀⠀⣶⠀
⢸⣿⣿⣿⣿⣿⣿⡿⢿⣿⡿⠟⢻⣿⣿⡟⠛⠛⠛⠉⠙⠛⠋⠀⠈⠉⠀⠈⠉⠁
⢸⣿⠿⠟⠋⠉⠀⢀⣾⡿⠉⠀⠈⠸⣿⣧⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠉⠁⠀⠀⠀⠀⠹⣿⣷⣤⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⠻⠃⠀⠀⠀⠀⠀⠀""")
water=(""" ⢀⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣾⣷⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⣼⣿⣿⣧⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⣾⣿⣿⣿⣿⣷⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⣾⣿⣿⣿⣿⣿⣿⣷⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⣾⣿⣿⣿⣿⣿⣿⣿⣿⣷⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⢠⣾⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣷⡄⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⢠⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⡄⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⢠⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⡄⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⢻⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⡟⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠈⢻⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⡟⠁⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠙⠻⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⠟⠋⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠉⠙⠛⠛⠛⠛⠋⠉⠀⠀⠀⠀""")

snake=("""⠀⢀⣀⣤⣴⢶⣾⣞⠒⠶⢤⣀⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢰⡟⢩⣇⠀⢛⣿⡟⠀⠀⠀⠙⢿⡲⢤⣀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠘⣿⡒⡳⠒⠚⠙⠒⠂⠀⠀⠰⡄⢹⡄⢟⢷⣄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⠉⢹⡿⠶⣶⣤⡤⠤⠤⠖⢿⠁⣹⣺⡾⠈⢷⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⡇⠀⠀⠘⣗⡒⠒⠒⢺⡏⣹⣽⡇⢰⠀⢳⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢸⠇⠀⠀⡄⢿⣉⠑⠒⢚⣏⣹⠉⡟⡞⢀⡎⡇⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣼⠀⠀⠀⢧⣾⣮⣉⠒⢺⠋⡟⢺⣷⠛⣟⡼⣿⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢠⡏⠀⠀⣇⣼⣾⠃⠈⠁⡏⢸⠷⣇⣼⠚⠋⠀⡟⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⣿⠀⣠⢀⣟⣡⡏⠀⠀⣸⠁⣿⣟⣩⡄⢀⠀⣸⠇⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢸⣿⣠⠿⣼⢛⡟⠀⠀⢠⠃⢸⣟⡽⣥⠷⡜⣶⡟⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢸⡇⢹⣶⢯⢯⣉⠒⠶⡞⣠⣿⢯⡴⢧⢼⣿⠏⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠘⣷⣾⣸⠻⢤⣈⠉⣻⠉⢠⣇⣾⣷⣿⠟⠁⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠘⣿⠃⠀⠀⠀⣰⠃⢀⡿⣻⣿⠟⠁⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⣼⠋⠀⠀⠀⢠⠇⢀⣾⠟⠋⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣼⠃⠀⠀⠀⠀⠀⢀⣾⠏⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢰⡏⠀⠀⠀⠀⠀⢀⣿⠏⢠⡿⣄⠀⠀⠀⠀⠀⠀⠀⠀⣀⣠⠴⠶⠶⠶⠤⣄⣀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢠⣿⠀⠀⠀⠀⠀⢀⣾⡏⠀⠀⠻⣝⠷⣄⣀⣀⣀⣤⠶⠛⠁⠀⠀⠀⠀⠀⠀⠈⢻⡙⢶⣄⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⣀⣀⣀⣀⣀⣀⠀⢸⡇⡀⠘⢦⣰⢃⣸⣿⠀⠀⠀⠀⠙⢷⣄⣀⣩⣥⡤⠤⠦⠦⠤⢤⣤⣤⣤⣴⡶⠏⠀⠀⠙⡆⠀⠀⠀⠀⠀
⠀⠀⠀⣠⡴⠞⠛⠉⢀⡠⠆⠀⠉⠙⢻⡇⠙⠢⣄⣿⣁⣼⣿⣤⠤⠤⠶⠛⠛⠉⠁⠀⣀⣀⣠⡤⠤⠤⠴⢶⠤⠴⠦⠤⣤⣀⣀⣴⡇⠀⠀⠀⠀⠀
⠀⢀⡞⠁⠀⠀⠀⢠⡎⠀⠀⠀⠀⠀⢸⡇⠲⣄⡀⠙⣇⣼⣿⠀⠀⠀⠀⣀⣤⠶⠚⠛⠉⠀⠀⠀⠀⠀⠀⠈⠙⠓⢦⡀⠀⠀⠙⠛⠦⣤⡀⠀⠀⠀
⢠⡟⠀⠀⠀⠀⠀⢸⣄⣤⣤⢤⣤⣀⣸⡇⠀⠀⠉⣋⣯⣸⣿⣤⡤⠞⠋⠁⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢹⡄⠀⠀⠀⠀⠀⠙⢧⡀⠀
⢸⡇⠀⠀⠀⠀⠀⠘⢿⣉⠀⠀⠀⠉⠛⣿⠤⢤⣀⠈⠙⣤⡿⣧⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣀⣀⣀⣤⣤⣤⣀⣸⣿⡄⠀⠀⠀⠀⠀⠘⣷⠀
⠸⣧⠀⠀⠀⠀⠀⠀⠀⠙⠛⠒⠒⠚⠛⢻⡆⠠⣄⣉⣉⣹⡼⢻⣧⠀⠀⠀⠀⠀⣀⣠⣤⠶⠟⠛⠋⠉⠀⠀⠀⠀⠀⠀⣹⡇⠀⠀⠀⠀⠀⠀⣹⠀
⠀⠘⢷⣄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢻⣄⠀⠀⠀⠀⠹⣍⠈⠳⣦⣴⡾⠿⠛⠉⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣠⡼⠋⠀⠀⠀⠀⠀⠀⢰⡿⡀
⠀⠀⠀⠙⠷⣤⣀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠻⣄⠀⠀⠀⠀⠈⠳⡄⠀⠉⠛⠲⠤⠤⣤⣀⣀⣤⠤⠤⠤⠔⠚⠋⠁⠀⠀⠀⠀⠀⠀⠀⢠⣿⠃⠀
⠀⠀⠀⠀⠀⠈⠙⠛⠶⠤⣤⣤⣤⣤⣤⣤⣴⠶⠿⢧⣄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⣴⡿⠁⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠉⠳⢦⣀⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣀⣤⣶⠟⠋⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⠙⠒⠲⠤⠤⢤⣄⣀⣀⣀⣀⣀⣀⣠⣤⣤⣤⡤⠶⠶⠛⠛⠉⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⣀⣀⠀⠀⠀⠀⠀⠀⠈""")


# water snake and gun project
# import random modules 
# import ramdon.randint function
# if ,elif,else conditions
# use return keyword
# input function 
# def function 
# 0=water
# 1=snake
# 2=gun


# import random model
import random
# create a function 
def fun(comp,user):
   # use if ,else and elif conditions 
   # create if condition
   if comp == user:
      print("Drow the game")
  # create if condition
   if comp==0 and user==2:
      print("win computer")
      print(water)
   # create if condition
   if comp==2 and user ==1:
      print("computer win")
      print("gun")
   # create else condition
   else: print("user win the game ")

# create the user variable 
user=int(input("Enter the value choice 0(water) 1(snake) 2(gun) \n"))
print(f"user:{user}")
# create the varible of computer 
comp=random.randint(0,2)
print(f"computer_user:{comp}")
# call function
fun(comp,user)






# 76 calculater project 
art=("""    _____________________
|  _________________  |
| | JO           0. | |
| |_________________| |
|  ___ ___ ___   ___  |
| | 7 | 8 | 9 | | + | |
| |___|___|___| |___| |
| | 4 | 5 | 6 | | - | |
| |___|___|___| |___| |
| | 1 | 2 | 3 | | x | |                                               
| |___|___|___| |___| |
| | . | 0 | = | | / | |
| |___|___|___| |___| |
|_____________________|
                   88                        88                     
                      88                        88              ,d     
                      88                        88              88     
 ,adPPYba, ,adPPYYba, 88  ,adPPYba, 88       88 88 ,adPPYYba, MM88MMM  
a8"     "" ""     `Y8 88 a8"     "" 88       88 88 ""     `Y8   88     
8b         ,adPPPPP88 88 8b         88       88 88 ,adPPPPP88   88     
"8a,   ,aa 88,    ,88 88 "8a,   ,aa "8a,   ,a88 88 88,    ,88   88,    
 `"Ybbd8"' `"8bbdP"Y8 88  `"Ybbd8"'  `"YbbdP'Y8 88 `"8bbdP"Y8   "Y888  
                                                        """)
print(art)
# create the functions with multiple operations 
def add(n1,n2):
    return n1+n2
def Subtraction(n1,n2):
    return n1-n2
def Multiplication(n1,n2):
    return n1*n2
def Division(n1,n2):
    return n1/n2
# create the dict key(all mathmecical operators and symbols )
operations={ "+" :add,
            "-":Subtraction,
            "*":Multiplication,
            "/": Division,}
def calculator():
     shouled_accumate=True
     while shouled_accumate:
         num1=float(input("what is your first no: "))
         for symbol in operations:
             print(symbol)
         operation_symbol=input("pick the operations symbol: ")
         num2=float(input("what is the next no:"))
         answer=(operations[operation_symbol](num1,num2))
         print(f"{num1} {operation_symbol} {num2} = {answer}")
         choice=input(f"type 'y' to countinue the calculation with{answer} or 'n' type to start the calculations:")
         if choice=="y":
             num1=answer
         else:
              shouled_accumate=False
              print(art)
              print( "\n"*2 )
              calculator()
calculator()








# project of blackjack
art="""88          88                       88        88                       88         
88          88                       88        ""                       88         
88          88                       88                                 88         
88,dPPYba,  88 ,adPPYYba,  ,adPPYba, 88   ,d8  88 ,adPPYYba,  ,adPPYba, 88   ,d8   
88P'    "8a 88 ""     `Y8 a8"     "" 88 ,a8"   88 ""     `Y8 a8"     "" 88 ,a8"    
88       d8 88 ,adPPPPP88 8b         8888[     88 ,adPPPPP88 8b         8888[      
88b,   ,a8" 88 88,    ,88 "8a,   ,aa 88`"Yba,  88 88,    ,88 "8a,   ,aa 88`"Yba,   
8Y"Ybbd8"'  88 `"8bbdP"Y8  `"Ybbd8"' 88   `Y8a 88 `"8bbdP"Y8  `"Ybbd8"' 88   `Y8a  
                                              ,88                                  
                                            888P"        """
print(art)
import random 
def deal_cards():
    cards=[11,2,3,4,5,6,7,8,9,10,10,10,10]
    card=random.choice(cards)
    return card

def compare(user_score, computer_score):
    """Compare user and computer scores."""
    if user_score == computer_score:
        return "Draw 😐"
    elif computer_score == 0:
        return "Lose, opponent has Blackjack 😭"
    elif user_score == 0:
        return "Win with a Blackjack 😎"
    elif user_score > 21:
        return "You went over 21. You lose 😭"
    elif computer_score > 21: 
        return "Opponent went over 21. You win 😎"
    elif user_score > computer_score:
        return "You win 😍"
    else:
        return "You lose 😭"
user_card=[]
computer_card=[]
user_score=-1
computer_score=-1
game_over=False
def calculate_score(cards):
    if sum(cards)==21 and len(cards)==2:
        return 0
    if 11 in cards and sum(cards)>21:
        cards.remove(11)
        cards.append(1)
    return sum(cards)
for _ in range (2):
    user_card .append(deal_cards())
    computer_card .append(deal_cards())

while not game_over:
   user_score= calculate_score(user_card)
   computer_score=calculate_score(computer_card)
   print(f"user_cards:{user_card} and user_score:{user_score}")
   print(f"computer_cards:{computer_card[0]}")
   if user_score ==0 or computer_score ==0 or user_score > 21:
       game_over=True
   else:
       user_should_deal=input("type 'y' to get another cards  and type 'n' pass:").lower()
       if user_should_deal=="y":
           user_card.append(deal_cards())
       else:
           game_over=True
while computer_score != 0 and computer_score < 17:
    computer_card.append(deal_cards())
    computer_score=calculate_score(computer_card)

    print(f"\nYour final hand: {user_card}, final score: {user_score}")
    print(f"Computer's final hand: {computer_card}, final score: {computer_score}")
    print(compare(user_score,computer_score))
  
           
    














