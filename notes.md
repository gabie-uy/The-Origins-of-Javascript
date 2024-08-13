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

## Variables

- **Variables** are used for storing data values
- Each variable has a name and they hold a value
- Usually written in **camelCase**, it is a naming convention in which the first letter of each word is capitalized, except for the first word.

To create or declare a variable:
- ``let`` is used for variables where the value will change.
- ``const`` is used for variables where the value will stay constant.

After the keyword, we need a variable name, an ``=`` sign, and a value:

        keyword name = value;

``=`` equal sign means assignment

Examples:

        const userId = 1618033988;
        let userName = "MonkeyGab";
        let progress = 0.75;
        let xp = 60;
        let verified = true;

- assigning the number value 1618033988 to the const variable userId.
- assigning the string value "MonkeyGab" to the let variable userName.
- assigning the number value 0.75 to the let variable progress.
- assigning the number value 60 to the let variable xp.
- assigning the truth value True to the let variable verified

## Data Types

- 8 Fundamentals (5 will be discussed below)

### Number

- Can be any integer or decimal number. It can be used to represent whole numbers, fractions or precise measurements.

        let year = 2023
        let age = 28
        let mealCost = 12.99
        const pi = 3.14
        const daysOfWeek = 7

### String

- Used for storing text or sequence of characters.
- Wrapped in double quotes ``" "`` or single quotes ``' '``

        let message = "good nite"
        let user = '@sonnynomnom'
        const company = "Codédex"

### Boolean

- ``bool``, stores a value that can only be either true or false
- In JavaScript, it's lowercased ``true`` or ``false``

        let hungry = true
        let lateToMeeting = false
        const earthIsFlat = false

### Null and Undefined

- Represents an absence of a value
- Written with ``null`` and ``undefined`` respectively (without double or single quotes)
- ``null`` represents the intentional absence of value
- ``undefined`` means the variable has been declared, but its value has not been assigned

        let newHire = null
        let startingDate = undefined

## Operators

**Arithmetic Operations**

1. ( + ) Addition
2. ( - ) Subtraction
3. ( * ) Multiplication
4. ( / ) Division
5. ( % ) Modulo (returns the remainder)

        let score = 0        // Declare score and initialize it

        score = 4 + 3        // score is now 7
        score = 4 - 3        // score is now 1
        score = 4 * 3        // score is now 12
        score = 4 / 3        // score is now 1.3333
        score = 4 % 3        // score is now 1

        console.log(score)   // Output: 1

**Example**:

        const pizza = 2.99
        const coke = 0.99

        let total = pizza + coke

        let tip = total * 0.2

        console.log(tip)     // Output: 0.796

This example can be shortened to:

        let tip = (pizza + coke) * 0.2

In JavaScript, parentheses have the highest order of operations.

## Exponents

- Superscript exponents and be denoted with ``**``

        let score = 0

        score = 2 ** 2      // score is 4
        score = 2 ** 3      // score is now 8
        score = 2 ** 4      // score is now 16
        score = 2 ** 5      // score is now 32

        console.log(score)  // Output: 32

**Note**: In the order of operations, exponents are calculated before multiplication/division and addition/subtraction.

## Control Flow

### if statement

- Tests a condition for truth and executes the code if it is true

        if (condition) {
                // Do something
        }

- If the condition is ``true``, then the statements within are executed. If the condition is ``false``, then nothing happens and the program continues on after the ``if`` statement.

        if (grade > 60) {
                console.log("You passed!");
        }

The if keyword is followed by a condition, grade > 60, inside a set of parentheses ( ).

- If the condition is true, the code inside the curly braces { } executes.
- If the condition is false, the code inside the curly braces is skipped.

### else statement

- An ``else`` clause can be optionally added to the end of an ``if`` statement.

        if (condition) {
                // Do something
        } else {
                // Do something else 
        }

- If the condition is ``true``, execute the code inside the ``if``.
- Else the condition is ``false``, execute the code inside the ``else``.

        if (grade > 60) {
                console.log("You passed.");
        } else {
                console.log("You failed.");
        }

### Comparison Operators

- (===) strict equal
- (!==) strict not equal
- (>) greater than
- (>=) greater than or equal
- (<) less than
- (<=) less than or equal

### else if

You can add an ``else if`` section between the ``if`` and ``else`` in your control flow! This gives your program more conditions to evaluate, besides just two.

        if (conditionA) {
                // Do this
        } else if (conditionB) {
                // Do this, instead
        } else {
                // Do this if none of the above are true
        }

Like the ``if`` statement, the code in an ``else if`` statement runs if its condition is true and the code in the rest of the ``if``/``else if``/``else`` statement is skipped.

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

## Logical Operators

**Logical operators**, also known as Boolean operators, combine and evaluate two conditions. They are ``&&``, ``||``, and ``!`` operators:

- The **AND** logical operator ``&&`` returns true if both conditions are true, and returns false otherwise.
- The **OR** logical operator ``||`` returns true if at least one of the conditions is true, and false otherwise.
- The **NOT** logical operator ``!`` returns true if the condition is false, and vice versa.

Examples:

        if (hunger > 4 && anger > 1) {
                console.log("Hangry");
        }

If the ``hunger`` variable is **greater than 4** and the ``anger`` variable is greater than 1, then the program prints "Hangry".

        if (coffee > 0 || bubble_tea > 0) {
                console.log("😊");
        }

If the ``coffee`` variable is greater than 0 or the ``bubble_tea`` variable is greater than 0, then the program prints a smiley face.

        if (!tired) {
                console.log("Let's code!");
        }

If the ``tired`` variable is not true, then the program prints "Let's code!"

| A | B	| A && B | A ll B |
|---|---|---|---|
| false | false	| false	| false |
| false	| true	| false	| true |
| true	| false	| false | true |
| true	| true	| true	| true |

## Loops

**Loops** are used to repeat a block of code based on a certain condition.

Example:

        let randomNumber = Math.floor(Math.random() * 10);

                while (randomNumber != 7) {
                console.log("Duck 🦆");
                randomNumber = Math.floor(Math.random() * 10);
        }

        console.log("Goose! 🦢");

## While Loops

The ``while`` loop uses a condition that is either ``true`` or ``false``.

        while (condition) {
                // Code here
        }

As long as the condition is ``true``, the code in the ``while`` loop will run. Otherwise, the loop ends when the condition becomes false.

