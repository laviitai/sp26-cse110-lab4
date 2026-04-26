### What was the bug?
the big is that num1 and num2 are strings, so they are being concatinated when they are added. 

### How would you fix it? 
to fix this bug I would edit the code so that it runs like this "let result = Number(num1) + Number(num2);" by having the Number identifier it will treat it as a number not a string