# OBJECT ITERATION

## GOAL

In this lab, you'll start to deal with objects that organize data more and more clearly. We'll start with a list of favorite books, but each book is keyed to a person's name.

For example, to print Zara's favorite book, you'd use the code `console.log(favoriteBooks["zara"])` or `console.log(favoriteBooks.zara)`.

Open up `script.js`, code out solutions to the challenges, and open the JavaScript console to see if the program is running correctly.

Once you finish your analysis the favoriteBook's object, there is a nested data structure that will require to use your knowledge of both lists and objects! Use the comments in `script.js` to help you out! 

![](https://media.giphy.com/media/BmmfETghGOPrW/giphy.gif)


## TIPS, EXAMPLES, & ANSWERS

Iteration for a dictionary is really similar to iteration for a list. Here's an example:
```javascript
var treatments = {
    "sunburn": "apply some aloe vera",
    "dehydration": "drink some water",
    "headache": "drink some water and consider taking a pain-reliever"
  }

//You're naming this internal variable (propery in this case). You can call it whatever you want, but the more descriptive your variable names, the easier they are to use.
for (var key in treatments) {

    console.log("If you're suffering from " + key + ", you should probably " + treatments[key] + ".") 
    // or with templateing
    console.log(`If you're suffering from ${key} you should probably ${treatments[key]}.`)
}

//Since the issue variable is only taking on the value of keys from the tratements dictionary, we need to use bracket notation to get the matching remedy for each issue.
```

If you need a boost, you can see answers to challenge 1. Solution to challenge 1:

  ```javascript

    //Reassign values for a key in a dictionary the same way we replace items in a list:
  
    favoriteBooks["jeff"] = "The Martian"
  
    // You can print it out to check whether it works by also including this line of debugging code:
  
    console.log(favoriteBooks["jeff"])
  
    //You can also access by using dot notation:
    
    console.log(favoriteBooks.jeff)
  ```