# Javascript Array Questions

- [Question 1: How do you check if a variable is an array in JavaScript?](#abc)
- [Question 2: How to insert an item into an array at a specific index (JavaScript)?](#abc)
- [Question 3: Remove Elements From A JavaScript Array](#abc)
- [Question 4: Javascript swap array elements by index](#abc)
- [Question 5: Find duplicate values in a array or Non unique array items](#abc)
- [Question 6: Remove duplicates from array or Uniques items array](#abc)
- [Question 7: Remove empty elements from an array in Javascript](#abc)
- [Question 8: Negative index array](#abc)
- [Question 9: Copy Array to another variable (Shalow and deep copy of an array](#abc)
- [Question 10: Sorting Array using methods and Sorting algorithms](#abc)
- [Question 11: Splice and Slice questions](#abc)

## Question 1: How do you check if a variable is an array in JavaScript?

```javascript
var arr = [];

// First approach
arr.constructor === Array // true

// Second approach
Array.isArray(arr);  // true

// Third approach
arr instanceof Array // true

// Fourth approach
Object.prototype.toString.call(arr) === '[object Array]'; // true
```

## Question 2: How to insert an item into an array at a specific index?

```javascript
// First approach: Using splice
var arr = [1,2,3,4,6];
arr.splice(4, 0, 5);
console.log(arr); // [1, 2, 3, 4, 5, 6]
```

## Question 3: Remove Elements From A JavaScript Array.

```javascript

```
https://love2dev.com/blog/javascript-remove-from-array/#clear-array

## Question 4: Javascript swap array elements by index.

```javascript
Array.prototype.swap = function (x,y) {
  var b = this[x];
  this[x] = this[y];
  this[y] = b;
  return this;
}

var arr = [1,2,3,4,6];

arr.swap(2,3) // [1, 2, 4, 3, 6]
```

## Question 5: Find duplicate values in a array or Non unique array items.

```javascript

```

## Question 6: Remove duplicates from array or Uniques items array.

```javascript

```

## Question 7: Remove empty elements from an array in Javascript.

```javascript

```

## Question 8: Negative index array.

You can assign arbitrary properties to an array (just like any other Object in JavaScript), which is what you're doing when you "index" the array at -1 and assign a value. Since this is not a member of the array and just an arbitrary property, you should not expect length to consider that property.

In other words, the following code does the same thing:

```javascript
var arr = [1,2,3];
arr[-1] = 4;
arr['x'] = "Suryansh"
console.log(arr); // [1, 2, 3, -1: 4, x: "Suryansh"]
console.log(arr.length); // 3
```

## Question 9: Copy Array to another variable (Shalow and deep copy of an array.
https://stackoverflow.com/questions/7486085/copy-array-by-value

| JS techniques used to copy array | Splice, Slice and Concat  | JSON (Parse and Stringify)  | $.extend, cloneDeep | Spread and Rest | 
| --- | --- | --- | --- | --- |
| Type 1: booleans, numbers and strings | Deep | Deep | Deep | --- |
| Type 2: Literal array and object | Shalow | Deep | Deep | --- |
| Type 3: Prototype objects | Shalow | Shalow | Deep | --- |

```javascript

```

## Question 10: Sorting Array using methods and Sorting algorithms.

```javascript

```

## Question 11: Splice and Slice questions.

```javascript

```
