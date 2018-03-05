# Overview

This assignment will give you practice creating HTML forms and using Javascript to process their contents to generate interesting or useful outputs. You will learn to:

* Create simple HTML forms with input elements and a button,
* Write Javascript functions that are used as event handlers,
* Incorporate conditional execution of code , and display results to the user, by dynamically changing the HTML page.

# Mad Libs

Many of us played with [Mad Libs](https://en.wikipedia.org/wiki/Mad_Libs) as kids. The idea is to ask someone — a friend, a victim — for some words, such as (1) a name, (2) a vehicle, (3) a restaurant, etc. Then, when you insert the words into a story, it yields a crazy result, because the choices were made without any idea of what the story would be. Here are screenshots of a Mad Libs page, both before and after a user has filled out the form and clicked the button:

![alt text](http://mysite.pratt.edu/~etrainer/Lab3/madlibs-1.png "Before")

![alt text](http://mysite.pratt.edu/~etrainer/Lab3/madlibs-2.png "After")

Your task will be to create a similar webpage to interactively play the Mad Libs game.

## Task 1: Creating the HTML Page

Create the file `madlibs.html` and give your new web page a header. Then:
* Create a `<form>` containing four `<input>` elements for the user to enter four missing words: for example, a noun for a name, a noun for an object, an adjective, and an adverb. You should only have one input for each of these words.
* It'll be useful to show a default value in all input elements to simplify your testing of the page.
* The form should also have a `<button>` element with an ID so that you can attach the event handler to it.
* There should also be a `<div>` element with an ID where the story will appear.


The requirements for the story and its appearance are:

* There must be exactly four input fields, but their meaning is up to you. Give them default values so that the form is easier to test.
* Define a new CSS rule in a `style.css` file to style all the user-supplied words, so that you can see which words were chosen when the story is displayed.
* You may use whatever color, font, etc. you wish - just make sure the inserted words are distinguishable from the rest of the story.
* The story must be at least four, but not more than six, sentences long (no longer!).
* There should be **8 missing words** in the story, so you will have to use some of the user-supplied words more than once. For example, the person's name was used three times in the sample story above. (Note that duplicated words are entered only once by the user!)
* Define HTML elements where your JavaScript code will display the values from the form. Think about how you'll target the correct element for the matching value.
* A story title should appear at the top of the story. This story title should include your own name (if you are Wendy, something like “Wendy's Crazy Mad Libs Story!”). Use your story title as the `<title>` for your HTML page as well.

The content of the story can be anything that you like — be creative!

## Task 2: Adding an Event Handler

In a `madlibs.js` file, define a function (name it whatever you like) that will process the form.  It should:
* Read the four form inputs, storing the values in variables.
* Copy the values into the story.

In your Javascript file, add code to attach the function to the button that will be clicked.

## Extra Credit

You can improve the appearance of the Mad Libs page for extra credit points by doing the following:

* Once the user clicks on the button, the form and its input fields should disappear, and the resulting story should be visible on the web page.
* Validate the input fields. If any input field is left blank, display an error message to the right of the input field **BEFORE** the user clicks "Tell Story."
* Use Semantic UI or Bootstrap to style input fields, buttons, and error messages.

## Advice
Keep the browser Console open at all times when you are writing and debugging JavaScript. Also, use the debugger and/or console.log() in your Javascript code, to make sure that your variables and expressions have the values you expect them to have.

## Grading Criteria

I'll use the following criteria to grade the homework:
* Homework was submitted on the server by the due date. Late penalties apply.
* Folders and files have the required names.
* All your files have comments at the top and as necessary interspersed in the code.
* Mad Libs page follows all requirements.
* There are no errors in the Javascript console.
* There are comments in the Javascript file to explain your code.