# Advanced Topics

## Functional Programming
> Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data — [Wikipedia](https://en.wikipedia.org/wiki/Functional_programming)

> Functions are pure when they are **deterministic** and cause no **side effects**. 

-   Deterministic = Same Arguments => Same Return **every time**.
-   No Side Effects = No Mutability

#### Advantages
1. Testing is much easier without the need to mock any data for functions to work on.
2. Pure functions are referentially transparent and can be memoized (cached into a hash map, I think) to increase application performance. 

## Refactoring JavaScript
#### Tips and Tricks 
- Return Early from Functions
- Cache Variables for Self-Evidency
- Check for Web APIs before implementing functionality

[Structure and examples from here - credit Andrew Healey](https://dev.to/healeycodes/refactoring-javascript-for-performance-and-readability-with-examples-1hec)

## Promise.all()
> Promise.all takes in a group of promises (typically an array) and returns a single promise representing the fulfillment of the group.

Promise.all is especially useful because it returns the promises in the same index order as the array.

Promise.all is dependent on all promises resolving correctly. A single promise break will return an error for the group.

### Cheat Sheet 
#### There are 5 static methods of Promise class:

1. Promise.all(promises) – waits for all promises to resolve and returns an array of their results. If any of the given promises rejects, it becomes the error of Promise.all, and all other results are ignored.

2. Promise.allSettled(promises) (recently added method) – waits for all promises to settle and returns their results as an array of objects with:
state: "fulfilled" or "rejected"
value (if fulfilled) or reason (if rejected).

3. Promise.race(promises) – waits for the first promise to settle, and its result/error becomes the outcome.

4. Promise.resolve(value) – makes a resolved promise with the given value.

5. Promise.reject(error) – makes a rejected promise with the given error.
Of these five, Promise.all is probably the most common in practice.

[Cheat Sheet From Here:](https://javascript.info/promise-api)