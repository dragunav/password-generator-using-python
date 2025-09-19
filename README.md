import random
letters =['a','b ' ,'c', 'd', 'e', 'f','g', 'h','i', 'j',' k', 'l', 'm', 'n', 'o',' p', 'q', 'r', 's', 't', 'u', 'v', 'w', 'x',' y' , 'z']
symbols = ['!','@','#','$','%','^','&','*','=']
numbers =['1','2','3','4','5','6','7','8','9','0']

print("\nWelcome to py password generator ==>> \n")
letter=int(input(" How many letters you want in password "))
symbol=int(input("\n How many symbols do you want in password "))
number=int(input("\n How many numbers do you want in password "))

password = []

for char in range (1,letter +1):
      password.append(random.choice(letters))

for char in range(1,symbol+1):
      password.append(random.choice(symbols))

for char in range(1,number+1):
      password.append(random.choice(numbers))

print(password) 
random.shuffle(password)   
pas_num=""
for char in password:
      pas_num += char

print(f"\npassword is = {pas_num}")
