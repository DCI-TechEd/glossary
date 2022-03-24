# General Programming Terms

## Abstraction

The act of reducing complexity in a computer program. It hides the complexity of a system behind a simpler API.

A simple example would be to separate and move some complex logic into a function. The function name would be the interface (API) to the logic.

## API (application programming interface)

An interface which allows communication to and from a system.

## Argument

An argument is a value passed as an input into a function.

##### Example

```
function foobar(name, date) {
}
```

In the above example, we can say the function "foobar" receives 2 arguments; name and date.

## Array

An array is an ordered collection of values. You can store multiple values in an array. An array has the datatype "object".

Each item in an array has a number attached to it, called a numeric index, that allows you to access it. In JavaScript, arrays start at index 0.

##### Example

`const names = [ 'Darwin', 'Luther' ];`

## Assignment

The act of giving a value to something, usually a variable. We use [assignment operators](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Assignment_Operators) to do this.

When we create a variable, we must assign it a value.

##### Example

`const age = 23`

In the above example, we are assigning the value `23` to the variable "age".

## Asynchronous

In JavaScript, the word asynchronous refers to operations (code) which is executed alongside other code. This is also known as non-blocking code, as execution of the asynchronous code does not prevent execution of other code.

This is opposite to synchronous code, which is executed sequentially (one after the other).

##### Examples of asynchronous code

Promises

```
new Promise((resolve) => {
  resolve();
});
```

Timeouts

```
setTimeout(() => {
  console.log('ding');
}, 200)
```

Intervals

```
setInterval(() => {
  console.log('ding');
}, 200)
```

async functions

```
async function asyncCall() {
  console.log('calling');
  const result = await resolveAfter2Seconds();
  console.log(result);
  // expected output: "resolved"
}
```

## Boolean

A datatype which can only have the values `true` or `false`.

Think of it like a simple light switch - a light switch can either be "on" (`true`) or "off" (`false`).

## Callback

A callback is any executable code that is passed as an argument to other code.

A callback is a function that is to be executed after another function (normally asynchronous) has finished executing — hence the name ‘call back’.

## Class (JavaScript)

In object-oriented programming, a class defines an object's characteristics. Class is a template definition of an object's properties and methods, the "blueprint" from which other more specific instances of the object are drawn.

## Closure

A closure is an inner function which has access to its outer environment while at the same time, maintaining its own private environment.

## Default (as in default behaviour)

The standard behaviour which will happen in a system, if no other behaviour is present to override it.

##### Example

You go to a coffee shop and you order a coffee. You only specify that it should be black. By "default" they put sugar in the coffee.
In order to override this behaviour, you must tell them if you want sugar or not.

## DOM (Document Object Model)

The Document Object Model represents the HTML on our page, as a hierarchy of objects.

With the DOM, we can interact with our HTML via these objects.

## Expression

Code which when executed, returns a single value. Expressions should be assigned to a container (variable) or the value will be lost.

##### The following examples are all expressions

- `2 + 2`

The above expression resolves to the number `4`

- `getValue()`

The above expression is the return from the function `getValue`

- `29 + calculateNumber()`

The above expression is the return from the function `calculateNumber` added to the number `29`

## Function

A function is a some code which can be called by other piece of code or by itself. When a function is called, arguments are passed to the function as an input, and the function can optionally return a value.

If no `return` statement is included in a function, that function will by default return `undefined`.

Functions usually have a name (this is known as the reference or identifier to the function).

Functions without a name are called _anonymous functions_.

## Hoisting

" the act of raising or lifting something "

No matter where they are declared, variable and function declarations are put into memory during the compile phase, meaning they can be referenced before they are declared. For example:

```
catName("Chloe");

function catName(name) {
  console.log("My cat's name is " + name);
}
```

In the above code, we can reference the function `catName` before it is declared because the compiler "hoists" or places the function `catName` into memory at compilation time.

```
console.log(a);
const a = 200;
```

In the above code, we get an error, because we initialise the variable `a` after we try to reference it.

## Instance (noun)

An object created by a constructor is an instance of that constructor.

For example, when we use the `new` keyword in JavaScript, the resulting value will be an instance.

## Instantiate (verb)

The act of creating an instance from a constructor.

## String

A datatype which contains a sequence of characters. In JavaScript, these can be enclosed inside single (') or double (") quotation marks.

##### The following examples are all valid strings in JavaScript

- `'hello'`

The above string uses single quotation marks.

- `"hello"`

The above string uses double quotation marks.

- `"2"`

The above is also a string. The string includes a number character. Please note, this is not the same as the number `2`.

## Method

A method is a function which is a property of an object. It is related to that object and usually describes some behaviour on that object.

## Number

A datatype which is a number, and can be used in calculations.

##### The following examples are all valid numbers in JavaScript

- `2`

- `2.3242`

## Object

A datatype which holds more complex data. We can (like an array) store multiple values in an object, except, (unlike an array) we can give those values names. These names are called keys.

Objects can also include functions which are called methods.

In JavaScript, objects are always contained inside brackets like these {}.

##### Example

```
const animal = {
    name: "Rex",
    age: 20
};
```

The above code shows a variable "animal" which is an object. This object has 2 keys - "name" and "age".

## Reference

A reference is our way to identify a value. For example, it can refer to a variable or a function. You can think of a reference as a name, which is a way of identifying something.
