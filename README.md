## ```Q1: What are the JavaScript Data Types?``` 
<details>
<summary>Answer</summary>

There are 7 data types in JS. These are:
1. All 6 premitive types 
2. Object: Complex data type that can store multiple premitive types. 
</details>

## ```Q2: What are primitive types in JS?```
<details>
<summary>Answer</summary>

> Primitive types are smallest and individual types those are unbreakable or can't be derived from any other data types. The 6 primitive types are:
1. undefined 
2. Boolean
3. Number
4. String 
5. BigInt
6. Symbol
7. null
</details>


## ```Q3: Are "undefined" and "null" all the same?```

<details>
<summary>Answer</summary>

> Not actually. Null represents the intentional absence of any object value whereas undefined refers to a variable when it's “value is not assigned”. undefined indicates the absence of a value, while null indicates the absence of an object.

Null is an explicit value and undefined is implicit.

```jsx
/// shows 'undefined' when value is not defined explicitely
let test;
console.log(test); /// result: undefined 
```

**```typeof(null)``` says object, it is a bug in JS**.

</details>


## ```Q4: Describe falsy and truthy values in JS.```

<details>
<summary>Answer</summary>

</details>

## ```Q5: Predict the results```
```javascript
1. console.log(10  + "20"); 
2. console.log(9 - "5");
3. 
3. console.log("Don't" + " " + "like");
4. console.log("abc" - "def"); // NaN
5. console.log("abc" - 10); 
```

<details>
<summary>Answer</summary>

1. Result 1: Number + String = String, the operation called concatenation
2. Result 2: Number - String = Number, **this is a bug in JavaScript**
3. Result : String + String = String, the operation called concatenation

### **```Weird JavaScript```**
In JavaScript, **Any data type - any data type = Number type**

```javascript
const str1 = " " - '5';
const str2 = " " - 5; 
console.log(str1, typeof str1); /// -5, " " - (Number in string) = Number
console.log(str2, typeof str2); /// -5, " " - Number = Number
```
</details>


## ```Q6: Boolean values```
In JavaScript, true represents 1 and false represents 0

```javascript
/// boolean addition, subtraction, value
const test1 = true + true;
const test2 = true + false;
const test3 = true - false;
const test4 = true - true;

const test5 = false + false;
const test6 = false + true;
const test7 = false - true;
const test8 = false - false;
```

<details>
<summary>Answer</summary>

Result: 
```typescript
2 number
1 number
1 number
0 number
0 number
1 number
-1 number
0 number
```
</details>

## ```Q7: What is NaN```

Predict the result
```jsx
let num;
const result = num * 10;
console.log(result);
```

<details>
<summary>Answer</summary>
&nbsp;

The answer is **```NaN```**, because of unexpected mathematical operation between undefined and a number. 

> **NaN** refers to **Not A Number**, produced when expected mathematical operation doesn't evaluates a number as result. Here are the reasons:
1. Invalid mathematical operations.
2. Converting non-numeric strings to numbers.
3. Performing operations where the result is not a real number.

> NaN often treated as an error, to these NaN values one can follow this conditional checking: 

```jsx
let number = NaN;
function test() {
  /// don't execute further if encounter NaN
  if (Number.isNaN(number)) return;

  console.log("I love someone, that is you!!");
}
test();
```
</details>

&nbsp;

### **Challenge**
```jsx
{
  let test = 10 * (true + true);
  console.log('result is: ', test);
}
```
<details>
<summary>Challenge result</summary>

```result is: 20```
</details>


