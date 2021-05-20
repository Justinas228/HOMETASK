a = 1
b = 2
print('Variable a and b', a, b)
string1 = input('Write your text here')
string2 = input('Write your name here')
number1 = input('Write your age here')
number2 = input('Write your cat age here')
print(f'Your text {string1} : Your name {string2} : Your age {number1} : Your cat age {number2} : ')

time = int(input('Write you time in seconds '))
hours = time // 3600
minutes = (time - hours * 3600) // 60
seconds = time - (hours * 3600 + minutes * 60)
print(f'Time in hours hh:mm:ss {hours} : {minutes} : {seconds} ')

n = int(input('Write you number '))
amount = (n + int(str(n) + str(n)) + int(str(n) + str(n)+ str(n)))
print('Amount of n + nn +nnn - %d'  % amount )

n = int(input("Enter you number "))
m = n % 10
n = n // 10
while n > 0:
    if n % 10 > m:
        m = n % 10
    n = n // 10
print('Max number', m)

Proceeds = int(input('Write your company proceeds '))
Cost = int(input('Write your comapny costs ' ))
print(f'Your company proceeds {Proceeds} : Your company costs {Cost} : ')
if Proceeds > Cost:
    print(f'Your company have  profit. Your company profitability is {Proceeds / Cost:.3f}')
Workers = int(input('How many wokers you have in company '))
print(f'Firm profit per employee {Proceeds / Workers:.3f}')
if Proceeds == Cost:
    print('Your company operates at zero')
else:
    print('Company is operating at a loss ')

a = int(input('You result KM' ))
b = int(input('Preferred result KM'))
days =  1
result_km = a
while result_km < b:
    a = a + 0.1 * a
    days += 1
    result_km = result_km + a
    print(f'Your result on %.d' % days)
