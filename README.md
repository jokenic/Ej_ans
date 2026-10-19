1) # ['red', 'blue', 'green', 'red', 'blue', 'blue']
mean colour = blue.

2) # blue is the most frequently worn.
   
3) sorting: ['blue' 'blue', 'blue', 'green', 'red', 'red' ]
   median = blue.
   
4) # variance.
   import statistics
   frequency = [3,2,1] #blue,red,green.
   print(statistics.variance(frequency)
   #output : 1.0.
   
5) # probability of picking red.
   total = Len(colours)
   red = colours.count('red')
   probability_red = reds / total
   print(probability_red) #output : 2/6 = 0.333.
   
6) import psycopg2
   # connect to DB
   conn = psycopg2.connect(database = "yours", user = 'user', password = 'pass', host = "localhost")
   cur = conn.cursor()
   # create table
   cur.execute(CREATE TABLE IF NOT EXISTS shirt_colours(colour TEXT, frequency INT)")
   # insert data
   for colour, frequency in [('blue', 3), ('red',2), ('green', 1)]:
   cur.execute("INSERT INTO shirt_colours VALUES (%S, %S)", (colour, frequency))
   conn.commit()
   conn.close()
   
7) # Recursive search for a number in a list
def recursive_search(last, target):
    if not last:
        return False
    if lst [0] == target:
        return True
        return recursive _search(last[1:], target)
numbers = [1,2,3,4,5]
print (recursive_search(numbers,3)) #output : True

8) # Generate random 4-digit binary number and convert to base 10.
import random
binary = ''.join(str(random.randint(0,1))
for I in range (4))
print(f"Binary: {binary}, Decimal: {int(binary,2)}") 

9) # Sum the first 50 Fibonacci numbers.
def Fibonacci_sum(n):
    a, b = 0,1
    total = 0
    for i in range (n):
        total += a
        a,b = b, a+b
    return total
print(fibonacci_sum(50))

    
