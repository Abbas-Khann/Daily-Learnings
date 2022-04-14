April 13 Learnings : 

- In CSS the width of an image given in percentage would work on the basis of the width of it's parent element. For example :

- If the width of the parent container is 50% and you should be setting the width of the image (child) to 100% in order to get the complete area of the container.

- But if you instead set the image's width to 50% it would take half of the area of it's parent aka the container in this case.

- Also it is preferred to have the parent's width to be much higher than 50% for smaller screens and then control the image through max-width and min-width properties.

- The em unit will inherit the size of the font from it's parent and make it twice as big every time you use it.

- Also don't use them they suck 

- The rem unit is a much better alternative and solution because it has a fixed size of 16px unless you haven't set up any font-size on the body of the html inside your css

- When display : flex is applied make sure the justify-content property's : space-between would only work if you content is less than 100% of the parent otherwise it won't effect the display at all.

- Also the align-items property behaves vertically by default so if flex-start is applied it would start from top to the capacity of the content towards bottom. 
- But if it's set to the centre then it would stay vertically centred