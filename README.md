### Assiut University Training - Newcomers

## Table of Contents

#### Sheet #1 (Datatypes - Conditions)
<li><a href="#Say_Hello_With_C++">Say Hello With C++</a></li>
<li><a href="#Basic_Data_Types">Basic Data Types</a></li>
<li><a href="#Simple_Calculator">Simple_Calculator</a></li>
<li><a href="#Difference">Difference</a></li>
<li><a href="#Area_of_a_Circle">Area_of_a_Circle</a></li>
<li><a href="#Digits_Summation">Digits_Summation</a></li>
<li><a href="#Summation_from_1_to_N">Summation_from_1_to_N</a></li>
<li><a href="#Two_numbers">Two_numbers</a></li>
<li><a href="#Welcome_for_you_with_Conditions">Welcome_for_you_with_Conditions</a></li>
<li><a href="#Multiples">Multiples</a></li>
<li><a href="#Max_and_Min">Max_and_Min</a></li>
<li><a href="#The_Brothers">The_Brothers</a></li>
<li><a href="#Capital_or_Small_or_Digit">Capital_or_Small_or_Digit</a></li>
<li><a href="#Char">Char</a></li>
<li><a href="#Calculator">Calculator</a></li>
<li><a href="#First_digit_!">First_digit_!</a></li>
<li><a href="#Coordinates_of_a_Point">Coordinates_of_a_Point</a></li>
<li><a href="#Age_in_Days">Age_in_Days</a></li>
<li><a href="#Interval">Interval</a></li>
<li><a href="#Sort_Numbers">Sort_Numbers</a></li>
<li><a href="#Float_or_int">Float_or_int</a></li>
<li><a href="#Comparison">Comparison</a></li>
<li><a href="#Mathematical_Expression">Mathematical_Expression</a></li>
<li><a href="#Two_intervals">Two_intervals</a></li>
<li><a href="#The_last_2_digits">The_last_2_digits</a></li>
<li><a href="#Hard_Compare">Hard_Compare</a></li>

#### Contest #1
<li><a href="#Winter_Sale">Winter_Sale</a></li>
<li><a href="#Memo_and_Momo">Memo_and_Momo</a></li>
<li><a href="#Next_Alphabet">Next_Alphabet</a></li>
<li><a href="#Ali_Baba_and_Puzzles">Ali_Baba_and_Puzzles</a></li>
<li><a href="#Interval_Sweep">Interval_Sweep</a></li>
<li><a href="#Adding_Bits">Adding_Bits</a></li>
<li><a href="#Katryoshka">Katryoshka</a></li>
<li><a href="#Lucky_Numbers">Lucky_Numbers</a></li>


<a id='Say_Hello_With_C++'></a>
### Say Hello With C++


```python
S = input()
print('Hello, ' + S)
```

<a id='Basic_Data_Types'></a>
### Basic Data Types


```python
vals = input().split()
vals[0] = int(vals[0])
vals[1] = int(vals[1])
vals[3] = float(vals[3])
vals[4] = float(vals[4])
for val in vals:
    print(val)
```

<a id='Simple_Calculator'></a>
### Simple_Calculator


```python
num1, num2 = input().split()
num1 = int(num1)
num2 = int(num2)
print('{} + {} = {}'.format(num1, num2 , num1 + num2))
print('{} * {} = {}'.format(num1, num2, num1 * num2))
print('{} - {} = {}'.format(num1, num2, num1 - num2))

```

     5 10
    

    5 + 10 = 15
    5 * 10 = 50
    5 - 10 = -5
    

<a id='Difference'></a>
### Difference


```python
# Read the input line and split it into four integers
A, B, C, D = map(int, input().split())

# Calculate the result of the equation
X = (A * B) - (C * D)

# Print the result with the required format
print(f"Difference = {X}")

```

     4 5 2 3
    

    Difference =  14
    

<a id='Area_of_a_Circle'></a>
### Area_of_a_Circle


```python
r = float(input())
pi = 3.141592653
print('{:.9f}'.format(pi * r**2))
```

     2
    

    12.566370612
    

<a id='Digits_Summation'></a>
### Digits_Summation


```python
n1, n2 = map(int, input().split())
print(f'{(n1 % 10) + (n2 % 10)}')
```

     12 13
    

    5
    

<a id='Summation_from_1_to_N'></a>
### Summation_from_1_to_N


```python
n = int(input())
print((n * (n + 1)) // 2)
```

     10
    

    55
    

<a id='Two_numbers'></a>
### Two_numbers


```python
import math

# Input: Read two integers A and B
A, B = map(int, input().split())

def strict_round(x):
    if x - math.floor(x) < 0.5:
        return math.floor(x)
    return math.ceil(x)

result = A / B
print(f'floor {A} / {B} = {math.floor(result)}')
print(f'ceil {A} / {B} = {math.ceil(result)}')
print(f'round {A} / {B} = {strict_round(result)}')

```

     10 4
    

    floor 10 / 4 = 2
    ceil 10 / 4 = 3
    round 10 / 4 = 3
    

<a id='Welcome_for_you_with_Conditions'></a>
### Welcome_for_you_with_Conditions


```python
n1, n2 = map(int, input().split())

if n1 >= n2: 
    print('Yes')
else:
    print('No')
```

     5 6
    

    No
    

<a id='Multiples'></a>
### Multiples


```python
n1, n2 = map(int, input().split())

if n1 % n2 == 0 or n2 % n1 == 0:
    print('Multiples')
else:
    print('No Multiples')
```

     6 24
    

    Multiples
    

<a id='Max_and_Min'></a>
### Max_and_Min


```python
nums = list(map(int, input().split()))
minimum = nums[0]
maximum = nums[0]
for n in nums[1:]:
    if n < minimum:
        minimum = n
    elif n > maximum:
        maximum = n

print(f'{minimum} {maximum}')
```

     10 2 3
    

    2 10
    

<a id='The_Brothers'></a>
### The_Brothers


```python
last_name1 = input().split()[-1]
last_name2 = input().split()[-1]
if last_name1 == last_name2:
    print('ARE Brothers')
else:
    print('NOT')
```

     ali kamel
     ali salah
    

    NOT
    

<a id='Capital_or_Small_or_Digit'></a>
### Capital_or_Small_or_Digit


```python
x = input()
if x.isdigit():
    print('IS DIGIT')
elif x.isalpha():
    print('ALPHA')
    if x.isupper():
        print('IS CAPITAL')
    else:
        print('IS SMALL')
```

     A
    

    ALPHA
    IS CAPITAL
    

<a id='Char'></a>
### Char


```python
x = input()
if x.isupper():
    print(x.lower())
else:
    print(x.upper())
```

     A
    

    a
    

<a id='Calculator'></a>
### Calculator


```python
import math

exp = input()
print(math.floor(eval(exp)))
```

     5/2
    

    2
    

<a id='First_digit_!'></a>
### First_digit_!


```python
n = int(input())

while n // 10 != 0:
    n //= 10

if n % 2 == 0:
    print('EVEN')
else:
    print('ODD')
```

     3569
    

    ODD
    

<a id='Coordinates_of_a_Point'></a>
### Coordinates_of_a_Point


```python
x, y = map(float, input().split())

if x == 0 and y == 0:
    print("Origem")
elif x == 0:
    print("Eixo Y")
elif y == 0:
    print("Eixo X")
elif x > 0 and y > 0:
    print("Q1")
elif x < 0 and y > 0:
    print("Q2")
elif x < 0 and y < 0:
    print("Q3")
else:
    print("Q4")

```

     4.5 -2.2
    

    Q4
    

<a id='Age_in_Days'></a>
### Age_in_Days


```python
n = int(input())

years = n // 365
months = (n % 365) // 30
days = (n % 365) % 30
print(f'{years} years')
print(f'{months} months')
print(f'{days} days')
```

     30
    

    0 years
    1 months
    0 days
    

<a id='Interval'></a>
### Interval


```python
n = float(input())

if n >= 0 and n <=25:
    print('Interval [0,25]')
elif n > 25 and n <=50:
    print('Interval (25,50]')
elif n > 50 and n <= 75:
    print('Interval (50,75]')
elif n > 75 and n <= 100:
    print('Interval (75,100]')
else:
    print('Out of Intervals')
```

     -25.2
    

    Out of Intervals
    

<a id='Sort_Numbers'></a>
### Sort_Numbers


```python
def quickSort(lst):
    if len(lst) < 2:
        return lst
        
    pivot = lst[0]
    smaller = [num for num in lst[1:] if num <= pivot]
    bigger = [num for num in lst[1:] if num > pivot]
    return quickSort(smaller) + [pivot] + quickSort(bigger)

nums = list(map(int, input().split()))
sorted_nums = quickSort(nums)

for n in sorted_nums:
    print(n)

print()

for n in nums:
    print(n)
```

     -1 5 2 -1 2
    

    -1
    -1
    2
    2
    5
    
    -1
    5
    2
    -1
    2
    


```python
nums = list(map(int, input().split()))

for n in sorted(nums):
    print(n)

print()

for n in nums:
    print(n)
```

<a id='Float_or_int'></a>
### Float_or_int


```python
n = float(input())

if n.is_integer():
    print(f'int {int(n)}')
else:
    integer_part = int(n)
    decimal_part = n - integer_part
    print(f'float {integer_part} {decimal_part}')

```

     5.9
    

    float 5 0.9000000000000004
    

<a id='Comparison'></a>
### Comparison


```python
exp = input()
if '=' in exp:
    exp = exp.replace('=', '==')
    
if eval(exp):
    print('Right')
else:
    print('Wrong')
```

     5 = 5
    

    Right
    


```python
import re

exp = input().strip()

# Replace a single '=' with '==', but avoid creating invalid expressions
exp = re.sub(r'(?<![=!<>])=(?!=)', '==', exp)

try:
    # Evaluate the expression
    if eval(exp):
        print('Right')
    else:
        print('Wrong')
except:
    print('Invalid expression')

```

<a id='Mathematical_Expression'></a>
### Mathematical_Expression


```python
exp = input()
if '=' in exp:
    exp = exp.replace('=', '==')

if eval(exp):
    print('Yes')
else:
    print(eval(exp.split('=')[0]))
```

     2 * 10 = 19
    

    20
    


```python
import re

exp = input().strip()

# Replace a single '=' with '==', avoiding issues with valid comparison operators
exp = re.sub(r'(?<![=!<>])=(?!=)', '==', exp)

try:
    # Evaluate the modified expression
    if eval(exp):
        print('Yes')
    else:
        # Evaluate and print the left-hand side of the original expression
        lhs = exp.split('==')[0]
        print(eval(lhs))
except:
    print('Invalid expression')

```

<a id='Two_intervals'></a>
### Two_intervals


```python
# Input: Two intervals [l1, r1], [l2, r2]
l1, r1, l2, r2 = map(int, input().split())

# Calculate the boundaries of the intersection
start = max(l1, l2)
end = min(r1, r2)

# Output the result
if start <= end:
    print(start, end)
else:
    print(-1)

```

     1 15 5 27
    

    5 15
    

<a id='The_last_2_digits'></a>
### The_last_2_digits


```python
nums = map(int, input().strip().split())

mult = 1
for num in nums:
    mult = (mult * num) % 100

print(f'{mult:02d}')
```

     10 10 10 10
    

    00
    

<a id='Hard_Compare'></a>
### Hard_Compare


```python
import math

n1, p1, n2, p2 = map(int, input().strip().split())

if p1 * math.log(n1) > p2 * math.log(n2):
    print('YES')
else:
    print('NO')
```

     4 2 5 2
    

    NO
    

## Contest #1

<a id='Winter_Sale'></a>
### Winter_Sale


```python
discount, price = map(int, input().split())
print(f'{price / (1 - (discount / 100)):.2f}')
```

     15 50
    

    58.82
    

<a id='Memo_and_Momo'></a>
### Memo_and_Momo


```python
a, b, k = map(int, input().strip().split())
if a % k == 0 and b % k == 0:
    print('Both')
elif a % k == 0:
    print('Memo')
elif b % k == 0:
    print('Momo')
else:
    print('No One')
```

     11 11 2
    

    No One
    

<a id='Next_Alphabet'></a>
### Next_Alphabet


```python
lower_alpha = input()
if lower_alpha == 'z':
    print('a')
else:
    ascii_value = ord(lower_alpha)
    print(chr(ord(lower_alpha) + 1))
```

     b
    

    c
    

<a id='Ali_Baba_and_Puzzles'></a>
### Ali_Baba_and_Puzzles


```python
from itertools import permutations

a, b, c, result = map(int, input().strip().split())

found = False
for operators in permutations(['+', '-', '*'], 2):
        if eval(str(a) + operators[0] + str(b) + operators[1] + str(c)) == result:
            print("YES")
            found = True
            break

if not found:
    print('NO')
```

     3 4 5 23
    

    YES
    

<a id='Interval_Sweep'></a>
### Interval_Sweep


```python
a, b = map(int, input().strip().split())

if a > 0 and abs(a - b) <= 1:
    print("YES")
else:
    print("NO")
```

     5 3
    

    NO
    

<a id='Adding_Bits'></a>
### Adding_Bits


```python
a, b = map(int, input().strip().split())
a_bin = format(a, 'b')
a_bin = (32 - len(a_bin)) * '0' + a_bin

b_bin = format(b, 'b')
b_bin = (32 - len(b_bin)) * '0' + b_bin


def parker_circuit(bin1, bin2):
    res = ''
    for b1, b2 in zip(bin1[::-1], bin2[::-1]):
        if (b1 == '0' and b2 == '0') or (b1 == '1' and b2 == '1'):
            res = '0' + res
        else:
            res = '1' + res
    return res

final_res = int(parker_circuit(a_bin, b_bin), 2)
print(final_res)
```

     6 9
    

    15
    


```python
a, b = map(int, input().strip().split())

# XOR directly simulates addition without carry, as Peter's flawed circuit does.
print(a ^ b)
```

     6 9
    

    15
    

<a id='Katryoshka'></a>
### Katryoshka


```python
eyes, mouths, bodies = map(int, input().strip().split())

# number of basic dolls (eyes = 1, mouths = 1, bodies = 1)
max_Katryoshkas = min(eyes, mouths, bodies)
eyes -= max_Katryoshkas
mouths -= max_Katryoshkas
bodies -= max_Katryoshkas

# number of additional dolls (eyes = 2, bodies = 1)
max_Katryoshkas += min(eyes//2, bodies)

print(max_Katryoshkas)
```

     90 24 89
    

    57
    

<a id='Lucky_Numbers'></a>
### Lucky_Numbers


```python
n = int(input().strip())
a = n // 10
b = n % 10
if b == 0:
    print('YES')
elif a % b == 0 or b % a == 0:
    print('YES')
else:
    print('NO')
```

     33
    

    YES
    
