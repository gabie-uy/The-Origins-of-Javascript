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

## Math.random()

In JavaScript, the ``math.random()`` method returns a random decimal number between 0 and 1.

Example:

        console.log(Math.random());
        console.log(Math.random());
        console.log(Math.random());

        0.0236966238022709
        0.7397680104909345
        0.4103022944399179

To get a random integer between 0 to 9:

        Math.floor(Math.random() * 10);

This is multiplying the decimal number by 10 and then rounding it down to the nearest integer with ``Math.floor()``.

