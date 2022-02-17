# Arrays

- List of items.
- Items can be of same or different data types.

#### Syntax-
	const array_name = [item1, item2, ...]; 

#### Example-
	const cars = ['BMW', 'Audi', 'Ford'];

## Accessing Array Elements

- Array elements can be accessed using index numbers.
- Index for arrays start from 0.

#### Example-
	const cars = ['BMW', 'Audi', 'Ford'];
	console.log(cars[0]);  // This will give 'BMW'

## Changing Elements of Array

- Elements of an array can be changed using the indexes.
- A new element can be assigned to the index of an array.

#### Example-
	const cars = ['BMW', 'Audi', 'Ford'];
	cars[1] = 'Toyota';  // This will assign 'Toyota' to the first index

## Nested Array

- Array within an array are nested arrays.

#### Example-
	const num = [1, [2, 3], 4];
	num[1][0];

- In the example, the whole sub-array '[2, 3]' belongs to the index 1.
- So, to access 2, we need to refer to 0th index of the sub-array which is at 1st index of the array.

## Length Property
- length property gives the length of an array, i.e, number of items in an array.

#### Syntax-
	array_name.length;

#### Example-
	const cars = ['BMW', 'Audi', 'Ford'];
	console.log(cars.length); // logs 3 as there are 3 items in the array

## Array Methods

### Push Method-
- Push method appends the new element to the array.

#### Example-
	const cars = ['BMW', 'Audi', 'Ford'];
	cars.push('Toyota'); // 'Toyota' is added to the end
	console.log(cars);

### Pop Method-
- Pop method removes an element from the end of the array.

#### Example-
	cars.pop();

### Shift Method-
- Shift method deletes first element of the array.
- Other elements shifts to a lower index.

#### Example-
	const cars = ['BMW', 'Audi', 'Ford'];
	cars.shift(); // 'BMW' is deleted 
	console.log(cars);

### Unshift Method-
- Unshift method adds the new element in the beginning of the array.
 
#### Example-
	const cars = ['BMW', 'Audi', 'Ford'];
	cars.unshift('Toyota'); // 'BMW' is deleted 
	console.log(cars);

### References-
- https://www.w3schools.com/js/js_array_methods.asp
- https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array

