- Today's Project Learnings(JS Day 39) : By giving a margin of -100vh to the first-page class we will enter the next page as soon as an event is clicked

- By putting all the insects in the and their names in a single span can help bring them in one box together

- To jump onto the next page through Javascript we should consider the screen in an array format and two classes with a similar name should be taken, also they should be accessed through querySelectorAll.
- Here's an example :
``` playBtn.addEventListener("click", ()=> {
    screen[0].classList.add("up")
})

```
- To get the image shown in the third page we need to get it's source in an empty object, And the reason why we take it in an empty object is so that we can use multiple properties so such as the alt , src etc
- Here's how we would get the image source : 
```
	  const image = item.querySelector("img")
        const src = image.getAttribute("src")
```
- In order to get the full width and height of a window So that it can be generated on a random place on the window we need to use 
```
const width = window.innerWidth
    const height = window.innerHeight
    const x = Math.random() * (width - 200) + 100
    const y = Math.random() * (height - 200) + 100
	// and return two values in an object since we have vertical and horizontal sides of the window
	
    return {x, y}
```




General Learnings: 

- Overflow property in CSS can be used to hide the overflow if wished by the developer
- Transition property in CSS can be used to create transitions and mini animations as well
- Object destructuring can be used to get multiple values from a function
- Conversion of seconds to minutes and then using it to call it in a certain amount of time should be done this way :
``` function increaseTime() {
    let min = Math.floor(seconds / 60)
    // console.log(min)
    let sec = seconds % 60
    // console.log(sec)
    if(min < 10) {
        min = `0${min}`
    }
    else {
        min = `${min}`
    }

    if(sec < 10) {
        sec = `0${sec}`
    }
    else {
        sec = `${sec}`
    }

    gameTime.innerHTML = `Time:${min}:${sec}`
    seconds++
}
```

Also make sure you have a global variable seconds set up to 0 before using this function