# GD1P01 Week 1, Pseudocode and Flowcharts

## Exercises

1. Use pseudo code to describe the process of making a cup of tea.
2. Use pseudo code to read two numbers, multiply them together and print their product.
3. Use pseudo code to read two numbers and print the largest number of the two.
4. Use pseudo code to read a number from the user and print whether the number is even or odd.
5. Uses pseudo code to read a number from the user. If the number is even it prints its square. If the number is odd, it prints its cube.
6. Use pseudo code to read three numbers from the user, sort them in ascending order and print the results.
7. Use pseudo code to print the largest number from 10 numbers stored in the memory.
8. Use pseudo code to calculate the average of 10 numbers read from the user.
9. Use pseudo code to print all the multiples of 3 between 1 and 100 (excluding both 1 and 100).
10. Use pseudo code to do the following:

    - Read numbers from the user till they enter ‘0’.
    - Calculate the average of the numbers.
    - Calculate the smallest and the largest number entered.
    - Print the average, minimum and maximum values.

### Question 1

```
PRINT "Boiling water"
waterTemp = 20 // Average room temp water

WHILE waterTemp < 100
    waterTemp += 1
ENDWHILE

PRINT "Adding tea bag"
teaBagTimer = 0

WHILE teaBagTimer < 60
    teaBagTimer += 1
ENDWHILE

PRINT "Removing tea bag"

PRINT "Adding milk"
maxMilkLevel = X
currentMilkLevel = 0

WHILE currentMilkLevel < maxMilkLevel
    currentMilkLevel += 1
ENDWHILE

PRINT "Tea complete"
```

<img src="https://github.com/Malachi-McEnroe/GD1P01-Week-1-Pseudocode-Flowcharts/blob/main/res/Question%201.drawio.png" alt="flowchart">

### Question 2

```
PRINT "Enter first number: "
READ num1
PRINT "Enter second number: "
READ num2

PRINT num1 * num2
```

### Question 3

```
PRINT "Enter first number: "
READ num1
PRINT "Enter second number: "
READ num2

IF num1 > num2
    PRINT num1
ELSE IF num2 > num1
    PRINT num2
ELSE
    PRINT num1 " is equal to " num2
ENDIF
```

### Question 4
```
PRINT "Enter a number: "
READ num

IF num % 2 = 0
    PRINT num " is even"
ELSE
    PRINT num " is odd"
ENDIF
```

### Question 5
```
PRINT "Enter a number: "
READ num

IF num % 2 = 0
    PRINT num * num
ELSE
    PRINT num * num * num
ENDIF
```

### Question 6
```
nums[3]

PRINT "Enter first number: "
READ nums[0]
PRINT "Enter second number: "
READ nums[1]
PRINT "Enter third number: "
READ nums[2]

WHILE i < 2
    j = i + 1
    temp1 = nums[i]
    temp2 = nums[j]

    IF nums[i] > nums[j]
        nums[i] = temp2
        nums[j] = temp1
    ENDIF
ENDWHILE

PRINT nums
```

### Question 7
```
nums[10] = [...]
largest = nums[10]

FOR num IN nums
    IF num > largest
        largest = num
    ENDIF
ENDFOR

PRINT largest " is the largest number"
```

### Question 8
```
nums[10]

PRINT "Enter a number: "
READ nums[0]

FOR i = 1 TO 9 STEP 1
    PRINT "Enter another number: "
    READ nums[i]
ENDFOR

total = 0

FOR num IN nums
    total += num
ENDFOR

avg = total / 10

PRINT avg " is the average"
```

### Question 9
```
FOR i = 1 TO 99 STEP 1
    IF i % 3 = 0
        PRINT i " is a multiple of 3"
    ENDIF
ENDFOR
```

### Question 10
```
nums[]

PRINT "Enter a number: "
READ nums[0]
i = 1

WHILE nums[i] != 0
    PRINT "Enter another number: "
    READ nums[i]
    i += 1
ENDWHILE

largest = nums[0]
smallest = nums[0]
total = 0

FOR num IN nums
    total += nums[i]
    
    IF num > largest
        largest = num
    ENDIF

    IF num < smallest
        smallest = num
    ENDIF
ENDFOR

avg = total / LENGTH(nums)

PRINT avg " is the average"
PRINT smallest " is the smallest number"
PRINT largest " is the largest number"
```


