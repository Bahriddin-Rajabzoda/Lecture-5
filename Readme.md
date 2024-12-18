![logo](logo1.png)

* TABLE OF CONTENTS

# 1. What is Array ?
# 2. What is method ?
# 3. Methods of Array
# 4. Mechanics in JS
# 5. Callbacks method

## In JavaScript, an array is a special type of object used to store multiple values in a single variable. 

    let fruits = ["Apple", "Banana", "Cherry"];

    console.log(fruits[0]); // Output: Apple

    fruits.push("Date");

    fruits.pop();

    console.log(fruits.length);
---

## In JavaScript, a method is a function that is associated with an object. Methods are used to perform actions on the data within the object. 

    let person = {
        firstName: "John",
        lastName: "Doe",
        fullName: function() {
            return this.firstName + " " + this.lastName;
        }
    };

    console.log(person.fullName());

## JavaScript arrays come with a variety of built-in methods that allow you to perform different operations on the array elements.

1. Push( ) - Adds one or more elements to the end of an array and returns the new length.

2. Pop( ) - Removes the last element from an array and returns that element.

3. Unshift( ) - Adds one or more elements to the beginning of an array and returns the new length.

4. Shift( ) - Removes the first element from an array and returns that elements.

5. ToString( ) - Returns a string representing the specified array and its elements.

6. IndexOf( ) - Returns the first index at which a given element can be found in the array, or -1 if it is not present.

7. Includes( ) - Determines whether an array includes a certain value among its entries, returning true or false.

8. Concat( ) - Merges two or more arrays and returns a new array.

9. Slice() - Returns a shallow copy of a portion of an array into a new array object selected from start to end.

10. Splice( ) - Changes the contents of an array by removing or replacing existing elements or adding new elements in place.

11. Join() - Joins all elements of an array into a string and returns this string.

12. ToReversed( ) - method in JavaScript is a new addition introduced in ES2023. It creates a new array with the elements in reverse order, without modifying the original array. This method is essentially a non-mutating version of the reverse( ) method.
---
## Syntax of method:
    1. push( ): let numbers = [1, 2, 3, 4, 5];
                numbers.push(6);
---
    2. pop( ): let numbers = [1, 2, 3, 4, 5];
               numbers.pop()
---
    3. unshift( ): let numbers = [1, 2, 3, 4, 5];
                   numbers.unshift(0)
---
    4. shift( ): let numbers = [1, 2, 3, 4, 5];
                 numbers.shift();
---
    5. toString( ): let str = fruits.toString();
---
    6. indexOf( ): let fruits = ["Apple", "Banana", "Cherry"];
                   let index = fruits.indexOf("Banana");
---
    7. includes( ): let hasApple = fruits.includes("Apple");
---
    8. concat( ): let moreNumbers = numbers.concat([6, 7, 8]);
---
    9. slice( ): let sliced = numbers.slice(1, 3);
---
    10. splice( ): numbers.splice(2, 1, 10);
---
    11. join( ): let joined = fruits.join(", ");
---
    12. toReversed( ): let fruits = ["Apple", "Banana", "Cherry"];
                       let reversedFruits = fruits.toReversed();
                       console.log(reversedFruits);
---
---
## Mechanics:
1. Mechanic destructuring - in JavaScript, destructuring is a convenient way of extracting values from arrays or properties from objects into distinct variables. This can make your code cleaner and more readable.
---
    let [a, b] = [1, 2];
    console.log(a);
    console.log(b);
---
2. Mechanic spread - In JavaScript, the spread syntax (...) allows an iterable, such as an array or string, to be expanded in places where zero or more arguments (for function calls) or elements (for array literals) are expected.
---
    let arr1 = [1, 2];
    let arr2 = [3, 4];
    let combined = [...arr1, ...arr2];
    console.log(combined); // [1, 2, 3, 4]
---
3. Mechanism rest - In JavaScript, rest parameters allow you to represent an indefinite number of arguments as an array. This is particularly useful when you want to work with functions that can accept any number of arguments.
---
    function sum(...numbers) {
        return numbers.reduce((acc, curr) => acc + curr, 0);
    }

    console.log(sum(1, 2, 3)); // 6
    console.log(sum(4, 5, 6, 7)); // 22
---
---

## In JavaScript, a callback is a function that is passed as an argument to another function and is executed after the completion of that function. This technique allows for more flexible and modular code, especially when dealing with asynchronous operations like network requests or file.
### In JS we have 6 callback method:
1. forEach( ) - method in JavaScript is used to execute a provided function once for each array element. It’s a convenient way to iterate over arrays without using a traditional for loop.
2. map( ) - method in JavaScript is used to create a new array by applying a provided function to each element of the original array. It’s a powerful tool for transforming data in arrays.
3. find( ) - method in JavaScript is used to locate the first element in an array that satisfies a provided testing function. If no elements satisfy the testing function, it returns undefined.
4. filter( ) - method in JavaScript is used to create a new array with all elements that pass a test implemented by a provided function. It’s a powerful tool for selecting elements from an array based on specific criteria.
5. reduce( ) - method in JavaScript is used to reduce an array to a single value by executing a provided function for each element of the array (from left to right). The result of each function call is stored in an accumulator, which is ultimately returned as the final result.
6. toSorted( ) - method is a relatively new addition to JavaScript, introduced in ECMAScript 2023. It creates a new array with the elements sorted in ascending order by default, without modifying the original array. This is particularly useful when you want to sort an array but keep the original array unchanged.
---

Syntax of callbacks method:

    1.  array.forEach(function(currentValue, index, array) {
    }, thisArg);
---
    2. let newArray = array.map(function(currentValue, index, array) {
    }, thisArg);
---
    3. let foundElement = array.find(function(element, index, array) {
    }, thisArg);
---
    4. let newArray = array.filter(function(element, index, array) {
    }, thisArg);
---
    5. let result = array.reduce(function(accumulator, currentValue, index, array) {
    }, initialValue);
---
    6. let sortedArray = array.toSorted(compareFunction);
---

![end](https://i.pinimg.com/originals/59/63/57/59635742174a5cb7d5583911b70cab31.gif)