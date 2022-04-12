April 12 Learnings(Day 41 JS): We concatenate the value in an empty string to the input box in the calculator through our else statement the reason is we should have an equal statement before the else statement that will use the inbuilt method of Javascript eval() which evaluates the value given in the parenthesis.

- Once It keeps on concatenating it will keep on executing the else statement and at some point the user have to press equal that's when the eval() method will be executed.
 
Here's an example : 
```
else if (buttonText === "=") {
            inputBox.value = eval(screenVal)
        }
```

And after this the concatenation else statement will be executed :
```
else {
            screenVal += buttonText
            inputBox.value = screenVal
        }
```


- General Learnings : 

-DEBUGGING IS THE MOST AMAZING THING IN THE HISTORY OF HUMANITY
- Also a life lesson: Webstorm is the best tool ever built for web devs

