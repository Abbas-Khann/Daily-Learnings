April 28 Learnings: 
Mappings in javaScript:


- Here are some examples to show how the map function works

/*
Challenge 1:
Given an array of numbers, return an array of each number, squared
*/

```
const nums = [1, 2, 3, 4, 5]
// -->       [1, 4, 9, 16, 25]
// Your code here
let squareNumbers = nums.map(item => {
    return item * item;
})
    console.log(squareNumbers)
```



/*
Challenge 2:
Given an array of strings, return an array where 
the first letter of each string is capitalized
*/
```
const names = ["alice", "bob", "charlie", "danielle"]
// -->        ["Alice", "Bob", "Charlie", "Danielle"]
// Your code here
   const UpperCaseNames = names.map(item => item[0].toUpperCase() + item.substring(1))
        console.log(UpperCaseNames)
```


/*
Challenge 3:
Given an array of strings, return an array of strings that wraps each
of the original strings in an HTML-like <p></p> tag.

E.g. given: ["Bulbasaur", "Charmander", "Squirtle"]
return: ["<p>Bulbasaur</p>", "<p>Charmander</p>", "<p>Squirtle</p>"]
*/
```
const pokemon = ["Bulbasaur", "Charmander", "Squirtle"]
// -->          ["<p>Bulbasaur</p>", "<p>Charmander</p>", "<p>Squirtle</p>"]
// Your code here

const pokemonParagraphs = pokemon.map(item => "<p>" + item + "</p>")

console.log(pokemonParagraphs)
```

Questions regarding Maps:


1. What does the `.map()` array method do?
It iterates through all the objects in an array or elements in an array


2. What do we usually use `.map()` for in React?

To iterate through elements and render them on the page dynamically


3. Why is using `.map()` better than just creating the components
   manually by typing them out?

Because We will be fetching data from API's and you will be working with dynamic data not statically typed data



