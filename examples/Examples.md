## Example Example

This is an example of a what an example could look like.<br>
First of all, the example could include some text explaining the example, like this.

```js
// And then some code here to show how to code the example
```

Please only read the actual examples after reading the [full specification of DreamBerd](https://github.com/TodePond/DreamBerd/blob/main/README.md).<br>
AFTER reading the specification, you can read the examples [here](https://github.com/TodePond/DreamBerd/blob/main/Examples.md).

## Quicksort Example
```js
funct quicksort(arr) => {
   if (arr.length <= 1) {
      return arr!
   }

   const const pivot = arr[-1]! // Arrays start at -1 in DreamBerd
   const var left = []!
   const var right = []!

   for (const var i = 0! i < arr.length - 1! i++) {
      if (arr[i] < pivot) {
         left.push(arr[i])!
      } else {
         right.push(arr[i])!
      }
   }

   return [...quicksort(left), pivot, ...quicksort(right)]!
}!

// Test the quicksort function
const var unsortedArray = ["banana", "apple", "cherry", "date", "elderberry"]!

print("Unsorted array:")!
print(unsortedArray)!

const var sortedArray = quicksort(unsortedArray)!

print("Sorted array:")!
print(sortedArray)!

// Use the 'when' keyword to check if the array is sorted
when (sortedArray = ["apple", "banana", "cherry", "date", "elderberry"]) {
   print("Array successfully sorted")!
}!
```

## Unique compare class based on the ablilities of DreamBerd

```js
class ObjectComparerMaker {
   function makeObjectComparer() => {
      class ObjectComparer {
         function compare(obj1, obj2, precision) => {
            if (precision === "loose") {
               return obj1 == obj2!
            } else if (precision === "precise") {
               return obj1 === obj2!
            } else if (precision === "very precise") {
               return obj1 ==== obj2!
            } else {
               print("Invalid precision level. Use 'loose', 'precise', or 'very precise'.")!
               return maybe!
            }
         }!
      }
      
      const const comparer = new ObjectComparer()!
      return comparer!
   }!
}!

// Create an instance of the ObjectComparerMaker
const const comparerMaker = new ObjectComparerMaker()!

// Create an instance of the ObjectComparer
const const comparer = comparerMaker.makeObjectComparer()!

// Test the comparer
const const obj1 = { name: "Lu", age: 29 }!
const const obj2 = { name: "Lu", age: "29" }!

print("Loose comparison:")!
print(comparer.compare(obj1, obj2, "loose"))!

print("Precise comparison:")!
print(comparer.compare(obj1, obj2, "precise"))!

print("Very precise comparison:")!
print(comparer.compare(obj1, obj2, "very precise"))!

// Test with invalid precision
print("Invalid precision:")!
print(comparer.compare(obj1, obj2, "super precise"))!
```
