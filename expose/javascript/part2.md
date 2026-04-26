## Part 2

### Question 1: What will happen at line 12 and why? If the code causes an error, explain why.
Line 12 prints 3. This is because the loop runs while i < 3, and after the final iteration i is incremented to 3 before exiting. Since var is function scoped, i is still accessible outside the loop, so it should report as 3.

### Q2: What will happen at line 13 and why? If the code causes an error, explain why. 
Line 13 should prints 150. This is because discountedPrice is declared with var, so it is still accessible outside the loop, and after the final iteration its value is from the last element, leading to the calculation 300 × 0.5 = 150.


### Q3: What will happen at line 14 and why? If the code causes an error, explain why. 
Line 14 will print 150. This is because finalPrice is declared with var and retains the value from the last loop iteration, which is 300 × 0.5 = 150.

### Q4: What will this function return? Give a brief explanation why. If the code causes an error, explain why.
The function returns [50, 100, 150]. This is because each price is multiplied by a 50 percent discount, and the results are pushed into the discounted array. No error occurs since all variables are properly defined and used within scope.

### Q5: What will happen at line 12 and why?  If the code causes an error, explain why (assume this function is being called like the others: discountPrices([100, 200, 300], 0.5)).
This will throw an error because i is declared with let inside the for loop, making it block scoped, so it is not accessible outside the loop where console.

### Q6: What will happen at line 13 and why? If the code causes an error, explain why.
Throws an error similar to Q5 because discountedPrice is block scoped as declared with let inside the for loop, so it is not accessible outside the loop.

### Q7: What will happen at line 14 and why? If the code causes an error, explain why.
This sucsessfully prints 150. This is because finalPrice is declared *outside* the loop with let, so it remains accessible after the loop and holds the value from the most recent iteration (300 × 0.5 = 150).

### Q8: What will this function return? Give a brief explanation. If the code causes an error, explain why. 
The function returns [50, 100, 150]. Each price is multiplied by 0.5 discount, and the results are added to the discounted array. No error occurs because all variables are correctly scoped with let.

### Q9: What will happen at line 11 and why? If the code causes an error, explain why.
This question will throw an error because i is declared with let inside the for loop, making it block scoped and inaccessible outside the loop.


### Q10:What will happen at line 12 and why? If the code causes an error, explain why.
Line 12 will print 3. This is because length is declared with const in the function scope as = prices.length, which is 3.

### Q11: What will this function return? Give a brief explanation. If the code causes an error, explain why.
The function returns [50, 100, 150]. Each price is multiplied by 0.5 and pushed into the array, all variables arre correctly scoped and acsessible, no errors thrown.

-------------------------------------------------------------------------------------
## Data Types

### Q12: Given the above Object, write the notation for: 
### A:Accessing the value of the name property in the student object
student.name

### B: Accessing the value of the Grad Year property in the student object
student['Grad Year']

### C: calling the function for the greeting property in the student object
student.greeting()

### D: Accessing the name property of the object in the Favorite Teacher property in student
student['Favorite Teacher'].name

### E: Access index zero in the array of the courseLoad property of the student object
student.courseLoad[0]

-------------------------------------------------------------------------------------
## Basic Operators & Type Conversion 

### Q13:
### A: '3' + 2
32
### B: '3' - 2
1
### C: 3 + null
3
### D: '3' + null
3null
### E: true + 3
4
### F: false + null
0
### G: '3' + undefined
3undefined
### H: '3' - undefined
NaN

### Q14:
### A: '2' > 1
true
### B: '2' < '12'
false
### C: 2 == '2'
true
### D: 2 === '2'
false
### E: true == 2
false
### F: true === Boolean(2)
true

### Q15: Difference between == and === operators:
== checks for equality with type conversions, meaning JavaScript will convert the values to the same type before comparing, while === checks for strict equality without converstion, meaning both the value and the type must match.

-------------------------------------------------------------------------------------
## Loops

#### Q16
answer in file "part2-question16.js"

-------------------------------------------------------------------------------------
## Functions

### Q17:
The result is [2, 4, 6]. The modifyArray function loops through [1, 2, 3] and applies the doSomething callback to each interger which multiplies each number by 2 and appends that to a new array.


-------------------------------------------------------------------------------------
## setInterval(), setTimeout(), clearTimeout()

### Q18:
answer in part2-question18.js

### Q19:
the output is: 1, 4, 3, 2. First, 1 and 4 are ran immediately. Then setTimeout(..., 0) logs 3 after the current call stack finishes, and finally setTimeout(..., 1000) logs 2 after another second.