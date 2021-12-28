# passgen
Password Generator App
import random

#A function do shuffle all the characters of a string
def shuffle(string):
  tempList = list(string)
  random.shuffle(tempList)
  return ''.join(tempList)

  #Main program starts here
  uppercaseLetter1=chr(random.randint(65,90)) #Generate a random Uppercase letter (based on ASCII code)
  uppercaseLetter2=chr(random.randint(65,90)) #Generate a random Uppercase letter (based on ASCII code)
  lowercaseLetter1=chr(random.randint(97,122))
  lowercaseLetter2=chr(random.randint(97,122))
  digit1=chr(random.randint(48,57))
  digit2=chr(random.randint(48,57))
  puntunationsign1=chr(random.randint(33,46))
  puntunationsign2=chr(random.randint(33,46))
  #....

  #Generate password using all the characters, in random order
  password = uppercaseLetter1 + uppercaseLetter2 + lowercaseLetter1 + lowercaseLetter2 + digit1 + digit2 + puntunationsign1+puntunationsign2
  password = shuffle(password)

  #Ouput
  print(password)
