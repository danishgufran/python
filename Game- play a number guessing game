#python code to play a number guessing game
#flags are used to break the main while loop
flag=0
while True:
  if(flag==1):
    break
  elif(flag==0):
   import time
   import random
   #set the interval of numbers in the game
   min=0
   max=10
   #set number of guesses allowed
   guess=5
   tries=guess
   #generating a random number
   number=random.randint(min,max)
   print('A RANDOM NUMBER IS GENERATED BETWEEN 0 & 10 AND YOU HAVE 5 GUESSES\n \t\t\t\t\tS T A R T')
   while guess>0:
     get=int(input('Enter a guess \n'))
     if(get<number):
       if(guess>0):
         #this function is executed if the guessed value is lower than the generated number
         guess-=1
         print("The guessed number is low\n\t\t\t\t\t\t\t\t you have",guess,"guesses left")
       else:
          break
     elif(get>number):
       if(guess>0):
         #this function is executed if the guessed value is higher than the generated number
         guess-=1
         print("The guessed number is high\n\t\t\t\t\t\t\t\t you have",guess,"guesses left")
       else:
          break
     else:
       #this function is executed if the guessed value is equal to the generated number
       guess-=1
       print('\n\nYou guessed the correct number in',(tries-guess),'tries')
       break
   while guess==0 or get==number:
     #display the generated number
     print('\n\tThe secret number was',number)
     sel=str(input('\n\t\t Press "Y" to play again else press "N"\n\t\t\t'))
     if sel=='n':
       print("\t\t\t\t BYE")
       #flag is set to break the main while loop
       flag=1
       break
     elif sel=='y':
       print("Game will restart in 3 seconds")
       print('...')
       time.sleep(1)
       print('..')
       time.sleep(1)
       print('.')
       time.sleep(1)
       #flag is 0 to repeat the main while loop
       flag=0
       break
