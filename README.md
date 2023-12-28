## ```Q1: What are the JavaScript Data Types?``` 

There are 7 data types in JS. These are:
1. All 6 premitive types 
2. Object: Complex data type that can store multiple premitive types. 


## ```Q2: What are primitive types in JS?```
> Primitive types are smallest and individual types those are unbreakable or can't be derived from any other data types. The 6 primitive types are:
1. undefined 
2. Boolean
3. Number
4. String 
5. BigInt
6. Symbol
7. null


## ```Q3: Are "undefined" and "null" all the same?```
> Not actually. Null represents the intentional absence of any object value whereas undefined refers to a variable when it's “value is not assigned”. undefined indicates the absence of a value, while null indicates the absence of an object.

Null is explicit and undefined is implicit.


## ```Q4: Describe falsy and truthy values in JS.```


## ```Q5: Predict the results```
```javascript
1. console.log(10  + "20"); 
2. console.log(9 - "5");
3. 
3. console.log("Don't" + " " + "like");
4. console.log("abc" - "def"); // NaN
5. console.log("abc" - 10); 
```

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


