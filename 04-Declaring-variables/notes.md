Variables as labeled containers that hold various types of data, such as numbers, strings, or objects.

## What is a variable?

A variable is a designated space in memory where data can be stored, accessed, and manipulated.

Each variable has a unique name, which distinguishes it from others.

## How to declare a variable?

- `let` defines a mutable variable, whose value you can change.

- `const` declares a constant variable, which prevents value overwriting

## Mutable variables

```javascript
let month = "November";
month = "December";

console.log(month); // December
```

Note : Variable names are case-sensitive: month differs from Month.

## Constants

```javascript
const language = "JavaScript";
language = "PHP"; // error
```

## Other ways to declare variables

Variables can also be declared with the keyword `var`.

This keyword served to declare variables before let and const were introduced in the ECMAScript 6 (ES6) standard.

```javascript
var age = 21;
```

Variables declared with let or const are limited to the block where they are defined.

In contrast, variables declared with var are accessible throughout the entire function, even outside the block where they are declared.

This can cause unintended variable pollution. Additionally, variables declared with var can lead to variable hoisting and potential bugs or errors due to accidental redeclaration.

Therefore, it's advisable to use let or const in modern JavaScript for more predictable behavior.

```javascript
age = 21; // Not good practice
```

## Best Practices

- Use const by default to declare variables. Switch to let only when you need to reassign the variable's value.

- Avoid using var, as it can lead to unexpected behavior due to its function scope and hoisting characteristics.

- Refrain from declaring variables without keywords, as this can inadvertently create global variables and lead to potential conflicts.
