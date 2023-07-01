# Fizz Buzz Solution

For numbers from 1.....n

1. Print "Fizz" if number is divisible by 3
2. Print "Buzz" if number is divisible by 5
3. Print "FizzBuzz" if number is divisible by 3 and 5
4. Else print the number itself.

```python
def fizzbuzz(n):
    for num in range(1, n + 1):
        if num % 3 == 0 and num % 5 == 0:
            print("FizzBuzz")
        elif num % 3 == 0:
            print("Fizz")
        elif num % 5 == 0:
            print("Buzz")
        else:
            print(num)

fizzbuzz(20)
```

To write a clean code and follow DRY (Don't Repeat Yourself) principle, following solution is way better.

```python
def fizz_buzz(num):
    for n in range(1, num + 1):
        output = ""
        if n % 3 == 0:
            output += "Fizz"
        if n % 5 == 0:
            output += "Buzz"
        if output == "":
            output += str(n)
        print(output)
        
fizz_buzz(20)
```

---

[Python Exercise](/Python/README.md)

---
