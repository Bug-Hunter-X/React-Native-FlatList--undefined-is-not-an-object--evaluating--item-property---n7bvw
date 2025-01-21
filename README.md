# React Native FlatList - undefined is not an object Error

This repository demonstrates a common error encountered when using `FlatList` in React Native:  `undefined is not an object (evaluating 'item.property')`.  This typically occurs when trying to access a property of an item in your data array that does not exist or is undefined.

The `Bug.js` file shows the problematic code, while `BugSolution.js` provides the corrected implementation. The issue stems from the dynamic styling applied within the FlatList item rendering and an attempt to access data properties that may be missing in certain items.

## How to reproduce:

1. Clone this repository.
2. Run `npm install`.
3. Run the app on your React Native environment. You should see the error in the console.

## Solution:

The solution involves adding proper null or undefined checks before accessing properties within the dynamic styles of the FlatList items.