### Question 1: What is printed by line 9? If the code returns an error, explain why.
"values added: 20"

### Question 2:What is printed by line 13? If the code returns an error, explain why. 
This will return an error as result is declared with var inside the if block. With this structure, results exists only in the function block

### Question 3 Why should you not use var? Explain why. 
You should not use var because it is function-scoped, not block-scoped, which can lead to weird bugs like we see in line 13. Additionally, var allows re-declaration, which can cause confusing errors.

### Question 4 What is printed by line 9? If the code returns an error, explain why. 
"values added: 20"

### 5. What is printed by line 13? If the code returns an error, explain why. 
This will produce an error once again, as result was declared with let inside the if block, so it is block-scoped and does not exist outside the if function.

### 6. What is printed by line 9? If the code returns an error, explain why.
this will cause an error because result was assigned as a const, so it can not be modified

### 7. What is printed by line 13? If the code returns an error, explain why. 
this may also crash because result is defined in the if statement, and the code will not be able to retrive this if it does not dive into the if function first (which crashes the code).
