1. Using loops take 10 inputs from user and find the average of all the numbers.
```js
Ans :- 
let sum = 0
let count = 0
for(let i = 0 ; i < 10 ; i++){
  let input = +prompt("Enter Inputs")
    sum += input
    count++
  
}
let avg = sum / count
console.log(avg)

> Using function

function getAvg(){
  let sum = 0
  let count = 0
  for(let i = 0 ; i < 10 ; i++){
    let input = +prompt("Enter Inputs")
    sum += input
    count++
}

  let avg = sum / count
  return `The Average is ${avg}`

}
getAvg()
```

2. What will be the output of the code below

```js
let i = 0;
while (i < 3) {
  println('hi');
  i++;
}
Ans :- It will throw an Reference error because we don't have the property of println
```

3. Write a function named `getEvenSum` that accepts a parameter `max`. Return the sum of all even numbers. The value of max should default to 10.
```js
Ans :- 
function getEvenSum(max = 10){
  let sum = 0;
  for(let i = 1 ; i <= max ; i++){
    if(i % 2 === 0){
    sum += i
    }
  }
    return sum
}
getEvenSum(100)
```

4. Write a function named `getOddSum` that accepts a parameter `max`. Return the sum of all odd numbers. The value of max should default to 10.
```js
Ans :- 
function getEvenSum(max = 10){
  let sum = 0;
  for(let i = 1 ; i <= max ; i++){
    if(i % 2 !== 0){
    sum += i
    }
  }
    return sum
}
getEvenSum(100)
```


5. Write a function named `getProductOfDigits` that accepts a parameter `num`. It returns the product of all the digits in the number.

```js
Ans :-
function getProductOfDigits(num){
  let product = 1
  while(num > 0){
    product = product * (num % 10)
    num = Math.floor(num / 10)
  }
  return `The product of your digits is ${product}`;
  while(num < 0){
    return `enter a valid input`
  }
}
getProductOfDigits(12)
```

- If the input value is less than 0 return `not a valid input`
- For example if the input is `123` output should be `6`.

6. What will be the output of the following code below in multiple conditions? Explain with reason?

```js
function check(num) {
  if (num > 5) {
    return 'Bigger than 5';
  }

  if (num < 5) {
    return 'Smaller than 5';
  }

  return num;
}

check(10); // 'Bigger than 5' Here the number 10 is bigger than 5 so it will return the output.
check(1); // 'Smaller than 5' Here the number 1 is smaller than 5 so it will return the output. 
check(5); // 5 Here the numberr is equaal to 5 so it will return the num 5
```

7. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === 'Arya') return 'You are arya';
  if (name === 'John') return 'You are john';
  return 'Who are you';
}

getOutput('Arya'); // 'You are Arya' Here we are checking the condition for name === 'Arya' so it will return the output 
getOutput('John'); // 'You are John'  Here we are checking the condition for name === 'John' so it will return the output 
getOutput(); // 'Who are you' Here we are returning the value to the function. Since there id no value inside the function it returns 'Who are you'
```

8. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === 'Arya') console.log('You are arya');
  if (name === 'John') console.log('You are john');
  return 'Who are you';
}

getOutput('Arya'); // output will be 'You are arya' but returns 'Who are you' since we know that the console doesn't store the value automatically and it always returns the return value.  
getOutput('John'); // output will be 'You are john' but returns 'Who are you' since we know that the console doesn't store the value automatically and it always returns the return value. 
getOutput(); // Here we are returning the value so it will returns the output 'Who are you'
```

9. Can a function have multiple return statement? Give one example if possible and explain the reason.
```js
Ans :-
No, A single function cannot have the multiple return statements. If there may be it will only return the first return statement
```

10. What is the difference between `for` loop and `while` loop. What are the different place you can use them? Explain with example.
```js
Ans :-
> `for` loop will accepts the 3 values that is the starting value, ending value which we want to end the loop, and the third on is to increase or decrease the value
Example :-
let sum = 0;
for(let i = 0 ; i < 10 ; i++){
  if(i % 2 === 0){
    sum += i
  }
} 
console.log(sum)
Example :-
let sum = 0 ;
let i = 0
while(i < 10){
  if( i % 2 === 0){
    sum += i
  }
  i = i + 1
}
console.log(sum)
```
