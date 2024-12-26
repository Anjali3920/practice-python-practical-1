# practice-python-practical-1
#prog 1
a,b,c = eval(input("enter value:"))
d = b**2-4 *a*c
r1 = (-b + (d)**0.5)/2*a
r2 = (-b - (d)**0.5)/2*a
if d >=0:
    print("roots are real",r1,r2)
else:
    print("roots are not real")

# program 2 
# prog 2 wap to accept a number 'n' to copute
#a check whether n is prime or not
n = eval(input("enter value:"))
if n>1:
   for i in range(2,n):
       if n%i == 0:
          print(n, "not a prime number")
          break
   else:
       print(n, "prime number")
else:
    print(n, "not a prime number")

# b
#prog 2
#b generate all prime no. till n
n = eval(input("enter value:"))
for num in range(1,n):
    if num > 1:
        for i in range(2,num):
            if num%i == 0:
             break
        else:
            print(num,end = ',')

#prog 3
# p3  create a pyramid of the character * and a reverse pyramid
n = int(input("enter the no. of rows"))
for i in range(n):
    for j in range(n-i-1):
        print(" ",end =" ")
    for j in range(2*i+1):
        print("*",end =" ")
    print()
for i in range(n):
    for j in range(i+1):
        print(" ",end = " ")
    for j in range(2*n-2*i-3):
        print("*",end =" ")
    print()

    # prog 4
    #Program 4. WAP that accepts a character and performs the following:
#a. print whether the character is a letter or numeric digit or a specialcharacter.
#b. if the character is a letter, print whether the letter is uppercase or lowercase.
#c. if the character is a numeric digit, prints its name in text #Code
character = input("Enter data")
if character >='A' and character<='Z':
    print("uppercase letter")
elif character >='a' and character<='z':
    print("lowercase letter")
elif character >='0' and character<='9':
    print("numeric digit")
    n = int(character)
    dict={0: 'zero', 1: 'first', 2: 'two', 3: 'three', 4: 'four', 5: 'five', 6: 'six', 7: 'seven', 8: 'eight', 9: 'nine'}
    print(dict[n])
else:
    print("special character")

  # prog 5
  #Program 5. WAP to perform the following operations on a string.
#1. find the frequecy of a character in a string.
#Code
string = "hello anjali to python"
character = input("enter a character ")
f = 0
for i in string:
    if i == character:
        f += 1
print("frequency of", character, 'is', f)



#2 reeplace a characte by anther character in astring
string = "hello anjali to python"
print(string.replace("h","t"))

#3 remove the first occurance of a character in the string
string = "hello anjali to python"
print(string[1:len(string)])

#4 remove the all occurence of a character
string = "hello anjali to python"
print(string[:0])



# p6
#Program 5. WAP to swap the first n characters of tau strings.
#Code
str1 = input("enter first string: ")
str2 = input("enter second string: ")
n1= int(input("enter no of character which is to be swap: "))
n = str1[:n1]
m = str2[:n1]
if n1 <= min(len(str1), len(str2)):
   print(str1.replace(n,m))
else:
    print(str2.replace(m,n))


# p7
#Program 7)write a function that accepts two string and returns the indices of all the occurences of the second string in the first string as a list. If the second string is not present in present in first string then it should return -1.
#code
def occurances(a,b):
 newlist =[]

 if b not in a:
   print(-1)
 else:
  i = 0
  while i< len(a):
   c=a.find(b,i)
   if c== -1:
     break
   i=c+ len(b)
   newlist.append(c)
  print(newlist)
a= input("enter first string;")
b= input("enter second string:")
occurances(a,b)



  
    
