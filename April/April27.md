April 26 Learnings (React Project: Day 54)

- The important concept of Props :

- Props help us in making functionalities dynamic.


Quiz questions for Props: 



1. What do props help us accomplish?

props are like parameters that can be used in passing in data dynamically


2. How do you pass a prop into a component?

```

<MyAwesomeHeader title="???" />

```




3. Can I pass a custom prop (e.g. blahblahblah={true}) to a native
   DOM element? e.g. ```<div blahblahblah={true}>``` If yes Why and if no then why not?
   
   
No, because the JSX we use to describe native DOM elements will
be turned into REAL DOM elements by React. And real DOM elements
only have the properties/attributes specified in the HTML specification.
(Which doesn't include properties like `blahblahblah`)




4. How do I receive props in a component?

```

function Name(prop) {
    return(
        <Contact 
            <img src="{props.image}" /> assuming image is already defined in the api or whatever hardcoded data.
        
        />
    )
}

```


5. What data type is `props` when the component receives it?

- Object



