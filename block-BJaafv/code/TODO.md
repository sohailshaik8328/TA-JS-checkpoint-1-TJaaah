1. What is the difference between the two `sum` function given below?

```js
// first
function sum(a, b) {
  return a + b;
}

// second
function sum(a, b) {
  console.log(a + b);
}
Ans :- 
> Well, the first function returns the value of the sum and it will be stored. But we are not calling the function so it wil show undefined
> The second function also do the sum expression and logs it. But it can't returns or stores the value in it. So, it will returns 'undefined'
```

2. If we store the returned value of both functions above in variable `first` and `second` what will be the value of `first` and `second`.
``` js
Ans :-
> In the first function the returned value will be stored in the variable 
> In the second function the value returns undefined and it will store it in the second variable called second.

```

3. What will be the output when you call above `sum` function (first) with three parameter like `sum(12, 24, 35)`. Explain why?
```js
Ans :-
> For, the first one the output will be '36'. Since, we have only two parameters and three arguments it will returns the first two arguments sum.
> For the second one also the output will be '36' but it returns the value undefined due to not returning the function duw to 2 parameters the JavaScript understands that it will take only 2 arguments and 3rd one will be ignored.
```

4. Can you store the first `sum` function in a variable named `add`. If yes why? If no why?
```js
Ans :-
YES, Because it's a variable and it was not been declared before and we can store it.
```

5. Declare a function named `sayHello` the accepts a parameter `name` and returns the name like `Hello Arya`.
```js
Ans :-
function sayHello(name){
  return `Hello ${name}`
}
sayHello("Arya")
```

6. What will be the output of the function below and why?

```js
let userName = 'John';

function showMessage() {
  let message = 'Hello, ' + userName;
  return message;
}

showMessage();

Ans :- output will be  "Hello, John"
> Because the variable username is outside the function and JavaScript finds the variable which we have given outside either inside and it returns the output
```

7. What will be the output for `Output1` `Output2` and `Output3` in the code below.

```js
let userName = 'John';

function showMessage() {
  let message = 'Hello, ' + userName;
  return message;
}

alert(userName); // "John"

showMessage(); // "Hello, John""

alert(userName); // "John"
```

8. What is a Anonymous Function give example of three functions.
```js
Ans :- 
> Anonymous functions are nothing but the functions which doesn't have the name of the function. Such as arrow functions also
> example-1 :- 
let sum = function (a, b){
  return a + b
}
> example-2 :-
let sum = (a, b) => a + b

> example-3 :- 
let sum = (a, b) => {
  return a + b
}
```

9. Can function declaration be a Anonymous Function? Explain
```js
Yes, It can be anonymous based on the requirement like it will be readable and the code decreases due to it and it is easy to write. 
```

10. Give 5 example of good naming convention for defining a function. You can read the details below to do that.

```md
Functions are actions. So their name is usually a verb. It should be brief, as accurate as possible and describe what the function does, so that someone reading the code gets an indication of what the function does.

It is a widespread practice to start a function with a verbal prefix which vaguely describes the action. There must be an agreement within the team on the meaning of the prefixes.

For instance, functions that start with "show" usually show something.

Function starting with…

"get…" – return a value,
"calc…" – calculate something,
"create…" – create something,
"check…" – check something and return a boolean, etc.
Ans :- 
example-1 :- 
function show(name){
  alert(name)
}
show("John")
example-2 :-
function get(firstName, lastName){
  return `${firstName} ${lastName}`
}
get("Tony", "Stark")
example-3
function calc(a, b){
  return a + b;
}
calc(2, 3)
example-4
function create(create_prompt_value){
  let create_prompt = prompt("enter what you want")
  return create_prompt
}
create()
example-5
fucntion check(a, b){
  if(a > b){
    return true
  }else{
    return false
  }
}
```
