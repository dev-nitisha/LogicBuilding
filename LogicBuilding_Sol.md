# Logic Building
## 1. Print numbers from n down to 1 in reverse order.
## 🧾 Code
```python
def num(n):
    while n > 0:
        print(n)
        n=n-1
  num(20)
```

## 2. Print all even numbers between 1 and 100.
## 🧾 Code
```python
def even(n):
    i = 1
    while i < n:
        if i % 2 == 0:
            print(i)
        i = i + 1
```
## 3. Print all even numbers between 1 and 100.
## Code
```python
def odd(n):
    i = 1
    while i < n:
        if i % 2 != 0:
            print(i)
        i = i + 1
```
## 4. Print the multiplication table of a given number from n × 1 to n × 10.
## Code
```python
def table(n):
    i = 1
    while i <= 10:
        s= i*n
        print(f"{i} x {n} = {s}")
        i=i+1
```
## 5. Calculate and print the sum of the first n natural numbers.
``` python
def nums(n):
   sum=0
   i=1
   while i<=n:
       sum=sum+i
       i=i+1
   return sum      
print(nums(10))
```
## 6. Calculate the sum of all even numbers from 1 up to n. 
``` python
def nums(n):
   sum=0
   i=1
   while i<=n:
       if i % 2 == 0:
           sum=sum+i
       i=i+1
   return sum      
print(nums(10))
```
## 7. Calculate the sum of all odd numbers from 1 up to n. 

``` python
def nums(n):
   sum=0
   i=1
   while i<=n:
       if i % 2 != 0:
           sum=sum+i
       i=i+1
   return sum      
print(nums(10))
```
## 8. Calculate and print the factorial of a given number
``` python
def fact(n):
    facto=1
    i=1
    while i<=n:
        facto=facto*i
        i=i+1
    return facto
    
print(fact(5))
```
### using Recursion(not preferred) - time complexity is O(n) but uses unesessary stack
```python
def fact(n):
   if n== 0 or n ==1:
       return 1
   return n*fact(n-1)
print(fact(5))
```
##  9. Find and print the product of all digits of a given number. 
```python
def prod(n):
    product = 1
    while n>0:
        product=product * (n%10)
        n= n//10
    return product
print(prod(2234))
```
##  10. Count and print the total number of digits in a given number. 
```python
def tdig(n):
    count = 0
    while n>0:
        count=count+1
        n= n//10
    return count
    
print(tdig(2234))
```
## 11.  Reverse the given number and print the reversed value.
```python
def rev(n):
    reverse = 0
    while n>0:
        num=n%10
        reverse = reverse*10+num
        n=n//10
    return reverse
    
print(rev(2234))
```
