# The Origins of III: Javascript

**Example:** 

``console.log("Hi");``

## Console Log

A **web console** is a feature in your browser that can run JavaScript code.

- ``console.log()`` is the output command
- The message to **display** is inside the parentheses ``()`` and surrounded by quotation marks, either single ``'`` or double ``''``

        console.log("👋 Howdy!");

**Note**: It's optional to include a ``;`` **semicolon** at the end of a line in JavaScript.

## Line by Line

- Javascript is run line by line

        console.log("🚌 Greyhound to New York");
        console.log("🕥 Departs at 9:30 am");

## Comments

### Single Line Comments

We can create a **single line** comment using ``//``, two forward slashes

    // Displaying a message

    // console.log("Nada");

    console.log("Hi"); // I'm a comment, too!

- The first line is just a comment and the program goes to the next line.
- The second line is also a comment, but with code that gets ignored.
- The third line begins with runnable code, and ends with a comment.

### Multi-line Comments

We can create a **multi-line** comment using ``/*`` to start the comment and ``*/`` to end the comment:

    /* This is commented out.
    console.log("Nada.")
    Yep! This is, too.
    console.log("Not displayed, either.")
    */