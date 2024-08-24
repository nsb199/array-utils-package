# Array Utils Package

This npm package provides a collection of utility functions for performing common operations on arrays. These functions are designed to simplify and speed up array manipulation tasks in JavaScript projects.

## Installation

To install this package, run the following command:

```bash
npm install array-utils-package
```

## Usage

After installing the package, you can import and use the provided utility functions in your project. Below is an example of how to use the package:

```bash
const arrayUtils = require('array-utils-package');

const numbers = [1, 2, 2, 3, 4, 5, 5, 6, 7];

console.log(arrayUtils.sum(numbers)); // Output: 35

console.log(arrayUtils.average(numbers)); // Output: 3.888888888888889

console.log(arrayUtils.max(numbers)); // Output: 7

console.log(arrayUtils.min(numbers)); // Output: 1

console.log(arrayUtils.unique(numbers)); // Output: [1, 2, 3, 4, 5, 6, 7]

console.log(arrayUtils.clear()); // Output: []

console.log(arrayUtils.chunk(numbers, 3)); // Output: [[1, 2, 2], [3, 4, 5], [5, 6, 7]]

const nestedArray = [1, [2, 3], [4, [5, 6]], 7];
console.log(arrayUtils.flatten(nestedArray)); // Output: [1, 2, 3, 4, 5, 6, 7]

const arr1 = [1, 2, 3];
const arr2 = [2, 3, 4];
console.log(arrayUtils.difference(arr1, arr2)); // Output: [1]

console.log(arrayUtils.intersect(arr1, arr2)); // Output: [2, 3]
```

## Functions

1. `sum(arr)`
   - Description: Returns the sum of all elements in the array.
   - Parameters: `arr` (Array): The array of numbers.
   - Returns: `number`: The sum of the array elements.

2. `average(arr)`
   - Description: Returns the average of all elements in the array.
   - Parameters: `arr` (Array): The array of numbers.
   - Returns: `number`: The average of the array elements.

3. `max(arr)`
   - Description: Returns the maximum value in the array.
   - Parameters: `arr` (Array): The array of numbers.
   - Returns: `number`: The maximum value in the array.

4. `min(arr)`
   - Description: Returns the minimum value in the array.
   - Parameters: `arr` (Array): The array of numbers.
   - Returns: `number`: The minimum value in the array.

5. `unique(arr)`
   - Description: Removes duplicate values from the array and returns a new array with unique elements.
   - Parameters: `arr` (Array): The array of values.
   - Returns: `Array`: A new array with unique elements.

6. `clear()`
   - Description: Clears all elements from the array (returns an empty array).
   - Parameters: None
   - Returns: `Array`: An empty array.

7. `chunk(arr, size)`
   - Description: Splits the array into chunks of a specified size.
   - Parameters: `arr` (Array): The array to be chunked.
   - Returns: `Array`: An array of chunks.

8. `flatten(arr)`
   - Description: Flattens a nested array into a single array.
   - Parameters: `arr` (Array): The nested array.
   - Returns: `Array`: A single flattened array.

9. `difference(arr1, arr2)`
   - Description: Returns an array of elements that are in the first array but not in the second.
   - Parameters: `arr1` (Array): The first array.
   - Returns: `Array`: An array of elements in `arr1` that are not in `arr2`.

10. `intersect(arr1, arr2)`
    - Description: Returns an array of elements that are common to both arrays.
    - Parameters: `arr1` (Array): The first array.
    - Returns: `Array`: An array of elements that are common to both `arr1` and `arr2`.

