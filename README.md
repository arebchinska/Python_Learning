# Python_Learning

print("Witaj, świecie!")
print("Jak masz na imię?")
myName = input()
print("Miło Cię poznać," + myName + ".") 
print("Liczba znaków w Twoim imieniu wynosi :")
print(len(myName))
print("Ile masz lat?")
myAge = input()
print("Za rok będziesz mieć  " +str(int(myAge)+1)+"  lat.")


EX1

a1,b1,a2,b2 = int(input()),int(input()),int(input()),int(input())

if b2>b1 and b1>a2 and a2>a1:
    print(a2,b1)
elif a1<b2 and a2<a1 and b2<b1:
    print(a1,b2)
elif b1==a2:
    print(b1)
elif b2==a1:
    print(a1)
elif (a1==a2 and b1<b2) or (a2<a1 and b1==b2) or (a1==a2 and b1==b2) or (a2<a1 and b1<b2):
    print(a1,b1)
elif (a1<a2 and b1==b2) or (a1==b1 and b2<b1) or (a1<a2 and b1>b2):
    print(a2,b2)
else:
    print("Pusty zbiór")
    
    
EX2

x = int(input())
if x == 0:
    print("zielony")
elif x >=1 and x <= 10:
    if x % 2 == 1:
        print("czerwony")
    else:
        print("czarny")
elif x >= 11 and  x <= 18:
    if x % 2 == 0:
        print("czerwony")
    else:
        print("czarny")
elif x >= 19 and x <= 28:
    if x % 2 == 0:
        print("czarny")
    else:
        print("czerwony")
elif x >= 29 and x <= 36:
    if x % 2 == 0:
        print("czerwony")
    else:
        print("czarny")
else:
    print("błąd wprowadzania")

EX3
a = input()
b = input()
if (a =="czerwony" and b == "niebieski") or (a == "niebieski" and b =="czerwony"):
    print("fiolet")
elif (a =="czerwony" and b == "żółty") or (a=="żółty" and b=="czerwony"):
    print("pomarańczowy")    
elif (a =="niebieski" and b == "żółty") or (a=="żółty" and b=="niebieski"):
    print("zielony")
elif a=="czerwony" and b=="czerwony":
    print("czerwony")
elif a=="niebieski" and b=="niebieski":
    print("niebieski")
elif a=="żółty" and b=="żółty":
    print("żółty")    
else:
    print("błąd koloru")
    
EX4

a = int(input())
b = int(input())
x = input()
if x == "+":
    print(a+b)
elif x == "-":
    print(a-b)
elif x == "*":
    print(a*b)
elif x == "/":
    if b==0:
        print("Nie można dzielić przez zero!")
    else:
        print(a/b)
elif x!="+" or x!="-" or x!="*" or x!="/":
    print("Nieprawidłowa operacja")
    
EX5

x = int(input()),int(input()),int(input()),int(input()),int(input())
print("Najmniejsza liczba =", min(x))
print("Największa liczba =", max(x))

EX6

x = int(input())
a = x%10
b = x%100//10
c = x//100

if min(a,b,c) + a == max(a,b,c):
    print("Ciekawa liczba")
elif min(a,b,c) + b == max(a,b,c):
    print("Ciekawa liczba")
elif min(a,b,c) + c == max(a,b,c):
    print("Ciekawa liczba")
else:
    print("Nieciekawa liczba")
    
EX7

p1, p2, q1, q2 = int(input()),int(input()),int(input()),int(input())
print(abs(p1-q1) + abs(p2-q2))

EX8

x1,y1,x2,y2 = float(input()),float(input()),float(input()),float(input())
p = sqrt((x1-x2)**2 + (y1-y2)**2)
print(p)

EX9

from math import *

x= float(input())
a = radians(x)
y = sin(a)+cos(a)+(tan(a)**2)
print(y)

EX10

from math import *

x = float(input())
y = ceil(x) + floor(x)
print(int(y))

EX11

a = float(input())
b = float(input())
c = float(input())
d = b**2-4*a*c
x1 = -b/(2*a)
x2 = ((-b + d**0.5)/(2*a))
x3 = ((-b - d**0.5)/(2*a))
if a != 0 and d == 0:
      print(x1)
elif a != 0 and d > 0:
      print(min(x3,x2), max(x3,x2), sep="\n")
else:
      print("Nie ma wyniku")

EX12

from math import *
n = int(input())
a = float(input())
s = (n*a**2)/(4*tan(pi/n))
print(s)

EX13
from math import *

a = float(input())
b = float(input())
print((a+b)/2)
print(sqrt(a*b))
print(2*a*b/(a+b))
print(sqrt((a**2+b**2)/2))

EX14

a = int(input())
b = int(input())
c = int(input())
if a>b and b < c and a >c:
    print(a,c,b, sep="\n")
elif a < b and b > c and a < c:
    print(b,c,a, sep="\n")
elif a>b and b < c and a < c:
    print(c,a,b, sep="\n")
elif a<b and b == c and a < c:
    print(c,b,a, sep="\n")
elif a>b and b < c and a == c:
    print(c,a,b, sep="\n")
elif a==b and b > c and a > c:
    print(a,b,c, sep="\n")
    
EX15
num1,num2,num3 = input(),input(),input()
a = (len(num2) + len(num3))/2
b = (len(num1) + len(num3))/2
c = (len(num1) + len(num2))/2
if (len(num1) == a) or (len(num2) == b) or (len(num3) == c): 
    print("YES")
else:
    print("NO")

EX16
a = input()
b = int(input())
for i in range(b):
    print(str(a))
    
EX17   
x = int(input())
for i in range(x):
    print("*"*19)
    
EX18
m = float(input())
p = int(input())
n = int(input())
for i in range(n):
    print(i+1,m)
    m += (m * p/100)

EX19
m,n = int(input()),int(input())
if m < n:
    for i in range(m,n+1,1):
        print(i)    
elif m > n:
    for i in range(m,n-1,-1):
        print(i)     
else:
    print(m)
    
EX20
m, n = int(input()), int(input())
for i in range(m,n+1):
    if i % 3 == 0 and i %5 == 0:
        print(i)
    elif i % 17 == 0:
        print(i)
    if i % 10 == 9:
        print(i)
 EX21
 n = int(input())
for i in range(1,11):
    m = n*i
    print(n , "x", i ,"=", m)

EX21
a, b = int(input()),int(input())
counter = 0
for i in range(a,b+1):
    if (i ** 3 % 10 == 4) or (i ** 3  % 10 == 9):
        counter = counter + 1
print(counter) 

EX22
n = int(input())
total = 1
for i in range(1,n+1):
    total = total * i
print(total)

EX23
n = int(input())
total = 0
for i in range(1,n+1):
    if (i**2 %10 == 2)or(i**2 % 10 == 5)or(i**2 %10 == 8):
        total = total + i
print(total)

EX24
n = int(input())
total = 0
for i in range(n):
    num = int(input())
    total = total+num
print(total)

EX25 (Napisz program, który oblicza wartość wyrażenia.)
from math import *
n = int(input())
total = 0
for i in range(1,n+1):
    total += 1/i
print(total-log(n))

EX26(Program powinien wyświetlać pojedynczą liczbę zgodnie ze stanem problemu.)
n = int(input())
total = 1
for i in range(1,n+1):
    total = total * i
print(total)

EX27 (Program powinien wydrukować iloczyn liczb niezerowych.)
total = 1
for i in range(0,10):
    num = int(input())
    if num != 0:
        total = total*num
print(total)

EX27 (Program powinien wypisać sumę wszystkich swoich dzielników do jednej liczby.)
n = int(input())
total = 0
for i in range(n,0,-1):
    if (n % i == 0):
        total += i
print(total)

EX28 (Program powinien wypisać pojedynczą liczbę sumy przemiennej)
n = int(input())
total = 0
for i in range(1,n+1):
    if i % 2 ==0:
        total -=i
    elif i % 2 !=0:
        total +=i
 print(total)
 
 EX29 (Program powinien wypisać dwie największe liczby, każda w osobnym wierszu.)
n = int(input())
max1 = 0
max2 = 0
for i in range(n):
    num = int(input())
    if num > max1:
        max2 = max1
        max1 = num
    if max2 < num < max1:
        max2 = num
print(max1, max2, sep = "\n")

EX30 (Program powinien wypisać ciąg „TAK”, jeśli wszystkie liczby są parzyste, a „NIE” w przeciwnym razie.)
counter = 0
for i in range(1,11):
    num = int(input())
    if num % 2 == 0:
        counter = counter + 1
if counter == 10:
    print("YES")
else:
    print("NO")

EX31(Program powinien wypisać terminy ciągu Fibonacciego oddzielone znakiem spacji.)
n = int(input())
a,b = 1,1
for i in range(n):
    print(a, end = " ")  
    a,b = b, a + b
    
EX32 (Program powinien wypisać sekwencję słów, każde słowo w osobnym wierszu.
x = input()
while x != "FINISH":
    print(x)
    x = input()
 
EX33 (Program powinien wypisać terminy podanej sekwencji.)
x = input()
while x != "FINISH" and x != "finish":
    print(x)
    x = input()

EX34 (Program powinien wypisać całkowitą liczbę terminów w podanej kolejności.
x = input()
total = 0
while x != "stop" and x != "enough" and x != "sufficiently":
    total += 1
    x = input()
print(total)

EX35 (Program powinien wypisać ciąg liczb całkowitych podzielnych przez 7.)
x = int(input())
while x % 7 == 0:
    print(x)
    x = int(input())

EX36 (Program powinien wypisać sumę wyrazów danego ciągu.)
x = int(input())
total = 0
while x >= 0:
    total += x
    x = int(input())
print(total)

EX37 (Program powinien wypisać liczbę piątek.)
x = int(input())
total = 0
while x >= 1 and x <= 5:
    if x == 5:
        total += 1
    x = int(input())
print(totaL)

EX38 (Program powinien wyświetlać minimalną możliwą liczbę wybitych monet do zapłaty.)
x = int(input())
total = 0

while x:
    total +=1
    if x >= 25:
        x -= 25
    elif x >= 10:
        x -= 10
    elif x >= 5:
        x -= 5
    elif x >= 1:
        x -= 1
print(total)

EX39 (Program powinien wyświetlać cyfry wpisanego numeru w kolumnie w odwrotnej kolejności.)
num = int(input())
while num:
    last_digit = num % 10
    print(last_digit)
    num = num // 10

EX40 (Program powinien wypisać liczbę zapisaną w odwrotnej kolejności.)
num = int(input())
while num:
    last_digit = num % 10
    print(last_digit, end = "")
    num = num // 10

EX41 (Program powinien wyświetlać maksymalne i minimalne cyfry wprowadzonej liczby (z objaśnieniem).)
num = int(input())
num1 = str(num)
print("Maximum", max(num1))
print("Minimum", min(num1))

EX42 (Program powinien wyprowadzać wartości określonych ilości w określonej kolejności:
suma jego cyfr;
liczba cyfr w nim;
iloczyn jego cyfr;
średnia arytmetyczna jego cyfr;
jego pierwsza cyfra;
suma jego pierwszej i ostatniej cyfry))

num = int(input())
total = 0
total1 = 0
total2 = 1
total4 = num % 10

while num:
    last_digit = num % 10
    total += last_digit
    total1 += 1
    total2 *= last_digit
    total3 = total/total1
    num1 = num
    num = num // 10
    total6 = total4+num1 
print(total, total1, total2, total3,num1,total6, sep = "\n")

EX43 (Program powinien wyświetlić swoją drugą (od początku) cyfrę.)
num = int(input())
while num > 9:
    last_digit = num % 10
    num = num // 10
print(last_digit)  

EX44 (Program powinien wypisać "TAK", jeśli numer składa się z tych samych cyfr, a "NIE" w przeciwnym razie.)
num = int(input())
num1 = str(num)
if max(num1) == min(num1):
    print("YES")
else:
    print("NO")
