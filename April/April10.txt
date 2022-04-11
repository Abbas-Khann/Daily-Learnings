April 10th learnings :

- In order to align an item vertically in CSS one can use the property of transform with translateY
- Now translateY takes a value inside such as translateY(-50%) etc and in this case it will push the element -50% on the Y-axis or in simpler words it will be pushed upwards by -50%

- getElementsBYClassName() gets the list of all the elements which have a similar class and returns them in an array format just like querySelectorAll 

- A new way to write for loops would be for of :
 Something like this: 
```
const names = ['Karl', 'John', 'Steve'];

for (let i of names) {
	console.log(i)
}

```
- firstly we will get the name of the variable which in traditional for loops would be i

- The CSS keyframes property works in a range of 0% to 100% and is used in an object format but will need a name just like a function:
For instance: 
```
@keyframes addKeyframes {
	0% {
	  opacity : 0%;
	}
	100% {

	opacity: 100%;

	}
}

```
- The name of the keyframes will need to be called like a function in the animation property for example :
```
.WhicheverClassYouWantToAddKeyframesTo {
	animation: keyframesName time
		In our case
	animation: addKeyframes 0.5s;
}
```
