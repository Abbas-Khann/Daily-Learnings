April 18 (JS project: 46 Learnings) :
- In order to change the body color from light mode to dark mode we just need to flip the color values in the state of variables.
- But since you will be flipping the values of more than one element on your page it's much better to use CSS variables for defining the values and properties.


General Learnings : Local Storage in the browser only works with strings so you can only pass values in a string format.
- It consists of a key and a value which should be specified in the code itself
- The key and the value can be used for comparison purposes and to maintain the current state of a website(mostly used in Dark mode)

- Here's how localStorage should be used

```
 	let variable = setItem("Key", "Value")

 // And in order to get the value you only need to pass the key 

	localStorage.getItem("Key")
```

- Now this can be used for comparison purposes in your code to keep track of the history even after the page is refreshed.


- To clear the localStorage
```
localStorage.clear()
```

- You could also say localStorage is nothing but a pair of string values that can be used for keeping the history but that's what we have learned so far.