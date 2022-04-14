April 14(Day 42 JS project) : If one wants to fetch data from an API with respect to it's id in the url and you want to make it dynamic you would have to run a loop in another function and iterate through them all and pass in the variable in the parameter: 

- Here's how :
```javascript
    let apiURL = `https://pokeapi.co/api/v2/pokemon/${id}`
    let response = await fetch(apiURL)
    let data = await response.json()
    console.log(data)
    // getData(data)
    render(data)
}

async function getID() {
    for (let i = 1; i <= 150; i++) {
        console.log(i)
       await getApi(i)
    }
}

getID()
```

- Everytime the loop runs a new id will be given and that's how we will dynamically generate an id into our function

- To make the code more dynamic we can also try creating every element of pokemon card from JS by using the createElement method.


General Learnings: 
- [understanding flex-direction]

- display:flex => creates columns and makes it flow in row direction with this behaviour (default behaviour)
    1. justify-content => behaves left to right (horizontally)
    && 
    2. align-items => behaves top to bottom (vertically)

-    But if we were to change flex-direction to column the behaviour would also change and now 

    1. justify-content => would behave top to bottom (vertically)
    &&
    2. align-items => would behave left to right (horizontally)