# python-Lab-2
programmeringsteknik lab 2

input function prints text between parentheses as a prompt to the person running the code and then waits for the user to respond and returns it as a string. The response line is placed as a value in the namn variable.
# {namn} varibeln blir svaret som skrivs efter promptet som en strin vilket är varför man måste använda f string för du kommer inte svara 'Denise'
# namn=input('what is your name?')
# print(f'welcome {namn}')

# # The input always returns the answer as a string, so if you want the answer to be a number you must convert it to a int or float.
# age=int(input('How old are you'))
# print(f'okey you are {age}')

# # Covert miles miles per gallon to liters per mile
# # to round to nearst decimal use round function
# mpg=float(input('Ange miles per gallon:'))
# lpm=10./(mpg*1.609/3.785)
# lpm=round(lpm,2)
# print(f'detta svarar mot {lpm} liter per mil')

# # skriv och kör ett program som läser i grader i fahrenheit och omvandlar till celcius
# fahrenheit=float(input('Hur varmt är det?'))
# celcius=(fahrenheit-32)/1.8
# celcius=round(celcius,1)
# print(f'detta omvandlas till {celcius} grader celcius')

# # Skriv och kör ett program som läser in i kronor(heltal),räntesats(flytttal)och år(heltal) och skriver ut kapitalet i ränta
# # fattar inte formeln
# startkapital=int(input('kapital'))
# ränta=float(input('ränta:'))
# år=int(input('antal år:'))
# slutkapital=startkapital*(1+ränta/100)**år
# print(f'Beloppet blir {slutkapital} kr')




# # Skriv och kör ett program som läser in två flyttal
# # Fattar inte hur man löser ekvationen
# import math
# p=float(input('p:'))
# q=float(input('q:'))
# disc=p*p - 4*q
# d=math.sqrt(disc)
# print('x1 = ', (-p + d)/2.0)
# print('x2 = ', (-p - d)/2.0)


 

# #Choose different paths depending on condition, for this you can use if statement
# # Ex. read in two numbers and write out which is bigger

# x=float(input('1st number'))
# y=float(input('2nd number'))
# if x > y: 
#     print('1st number is bigger than 2nd number')
# else:
#     print('2nb number is bigger or x and y are equal')
    


# Grenarna kan också innehålla else och if och då är det bättre att använda elif
# x=-0
# if x > 0:
#     print('positiva fallet')
# elif x==0:
#     print('fallet 0')
# else:
#     print('negativa fallet')
# print('efter alla fall')
#utan elif hade man behövt definiera både else och if under else om x<0. Nu behöver vi bara definiera else efter elif.

#Logiska uttryck = uttryck som kan vara sant eller falsk och kallas för bool and the two values are written True and False.
#The conditions in the if statements above are examples of logical expressions.
# == lika
# != ej lika
# < mindre än
# <= mindre än eller lika
# > större än
# >= större än eller lika
#Operanderna måste vara jämförbara, båda tal eller strängar exempelvis. 
#and or och not är också logiska operander.
#Exemple för satsen är teenager = > 12 < 20 och variabeln teenager till True om åldern stämmer. 
# day="onsdag"
# if day == "lördag" or day == "söndag":
#     print("Helg")
# else:
#     print("Vardag")

#While satsen: När man vill upprepa en följd av satser flera gånger kallas det för en loop eller slinga. While loopen kan vi använda sålänge ett visst condition är sant.
# n är en factorial vilket innebär att den multiplicerar med nästkommande tal 1*2*2... upp till värdet du ger n som måste vara en positiv int.
#prod är en variabel som ackumulerar produkten och variabeln i räknar antalet.
#koden betyder att sålänge i är mindre eller lika med n så loopar den så många gånger som värdet av n.
# print('beräkning av n')
# n=int(input('ange n:'))
# prod=1
# i=1
# while i<=n:
#     prod*=i
#     i+=1
# print(f'{n} = {prod}')

#Exempel: läs in tal till en lista, be användaren mata in positiva tal och spara dem i en lista
# numbers=[] #En tom lista
# print('mata in positiva tal. avbryt med 0')
# x=int(input('första:'))
# while x>0:
#     numbers.append(x) #adds the number to the end of the list
#     x=int(input('andra:'))
# print('inmatad lista: ',numbers)

#normalt avslutas en while-loop när villkoret blir falskt men man kan breaka det fast villkoret stämmer. 
# import random #paket med slumptalsfunktioner
# number = random.randint(1,100) #välj ett slump int nummer mellan 1-100
# while True:
#     guess = int(input('guess umber:'))
#     if guess < number:
#         print('too small')
#     elif guess > number:
#         print('too big')
#     else:
#         print('correct')
#         break

# exercise 1.
# numbers = []
# print('give numbers, stop with 0')
# x=int(input('first:'))
# while x > 0:
#     numbers.append(x) 
#     x=int(input('next:')) 
# print('list:', numbers)
# n = 0 # n accumulates the result
# i = 0 # i = element(index) i listan börjar alltid på 0 i python
# while i < len(numbers): #len is a function that returns the number of items in an object. Så detta betyder att så länge indexet i listan är lägre än antalet objekt i listan fortsätter loopen för att gå igenom hela listan
#     if numbers[i] % 2 ==0:
#         n += 1 # lägger till ett jämnt nummer i antalet jämna nummer
#     i += 1 # går vidare till nästa element i listan
# print(n, 'even numbers')

# exercise 2.
# print('give a positive number')
# x=float(input('positive number:'))
# tries = 1
# while x <= 0:
#     x = float(input('try again:'))
#     tries += 1 #varje gång while loopen startas igen läggs det till ett försök till tries
# if tries > 3:
#     print('Finally')

#Exercise 4.
# import random #paket med slumptalsfunktioner
# number = random.randint(1,10) #välj ett slump int nummer mellan 1-100
# guess = int(input('guess umber:'))
# while guess != number:
#     if guess < number:
#         print('too small')
#     elif guess > number:
#         print('too big')
#     guess = int(input('guess umber:'))
# print('correct')

#For-loops is another way to repeat code. 
# sum = 1
# for i in range(6): # vi sätter värdet av elementen till i ett och ett
#     sum = sum + i
#     print(sum)

# prod = 1
# for i in range(6):
#     prod *= (i + 1)
#     print(prod)

# for variable in lista: "variable will successively assume the lists different values"
# firstnames = ['Bo','Eva','Ola']
# surnames = ['Ek', 'Strand']
# result = []
# for fn in firstnames:
#     for sn in surnames:
#         result.append(fn + ' ' + sn) # för varje fn går kod igenom alla sn och adderar alla möjliga outcomes till resultat.
# print(result)

list= [1,2,3,4,5,6]
for l in list:
    for i in range(l):
        print('*',end='')
    print()
