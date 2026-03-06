# Assignment-07
# Array Methods()

## 1. Using map()
Given the following array:
const numbers = [1, 2, 3, 4, 5];
Task:
Create a new array where each number is doubled.
Expected Output:
[2, 4, 6, 8, 10]
```
const numbers = [1, 2, 3, 4, 5]
const doubled = numbers.map(num => num * 2)## 
console.log(doubled);

```
## 2. Using filter()
const ages = [12, 18, 25, 10, 30, 16];
Task:
Create a new array containing only ages 18 and above.
Expected Output:
[18, 25, 30]

```
const ages = [12, 18, 25, 10, 30, 16];
const arr = ages.filter((item) => {
    return item >= 18
})
console.log(arr);

```
## 3. Using reduce()
const prices = [100, 200, 300, 400];
Task:
Find the total sum of all prices.
Expected Output:
1000
```
const prices = [100, 200, 300, 400];
const total = prices.reduce((sum, price) => sum + price)
console.log(total);

```
## 4. Using find()
const users = [
  { id: 1, name: "John" },
  { id: 2, name: "Jane" },
  { id: 3, name: "Jack" }
];
Task:
Find the user with id: 2.
Expected Output:
{ id: 2, name: "Jane" }

```
const users = [
    { id: 1, name: "John" },
    { id: 2, name: "Jane" },
    { id: 3, name: "Jack" }
];

const user = users.find(u => u.id === 2);

console.log(user);

```
## 5. Using some() and every()
const scores = [80, 90, 70, 60, 50];
Tasks:
•	Check if at least one score is below 60.
•	Check if all scores are above 40.
```
const scores = [80, 90, 70, 60, 50];
console.log(scores.some((item) => item < 60));
console.log(scores.every((item) => item > 40));
```
## 6. Using includes()
const fruits = ["apple", "banana", "mango", "orange"];
Task:
Check if "mango" exists in the array.
```
const fruits = ["apple", "banana", "mango", "orange"];
const hasMango = fruits.includes("mango");
console.log(hasMango);
```
## 7. Using sort()
const numbers = [10, 5, 40, 25, 100];
Task:
Sort the numbers in ascending order.
Expected Output:
[5, 10, 25, 40, 100]
```
const numbers = [10, 5, 40, 25, 100];
numbers.sort((a, b) => a - b);
console.log(numbers);
```
## 8. Combination Problem (filter() + map())
const products = [
  { name: "Laptop", price: 1000 },
  { name: "Phone", price: 500 },
  { name: "Tablet", price: 700 },
  { name: "Monitor", price: 300 }
];
Task:
Get the names of products that cost more than 600.
Expected Output:
["Laptop", "Tablet"]
```
const products = [
    { name: "Laptop", price: 1000 },
    { name: "Phone", price: 500 },
    { name: "Tablet", price: 700 },
    { name: "Monitor", price: 300 }
];

const expensiveProducts = products
    .filter(product => product.price > 600)
    .map(product => product.name);
console.log(expensiveProducts);
```
