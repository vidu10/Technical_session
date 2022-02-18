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
	
### Map Method-
- Map method executes the function for each element of an array.
- It takes a function as an argument.
- The original array remains same and it gives new array as a result.
#### Syntax-
	array_name.map(function_name);
#### Example- 
	const numbers = [65, 44, 12, 4];
	const newArr = numbers.map(multiply)

	function multiply(num) {   // takes each element of the array 'number' and multiply by 10
	  return num * 10;
	}

### Filter Method-
- Filter method creates a new array of elements that passes a function given to it.
- A function is provided as an argument to the filter method.
#### Example-
	const ages = [32, 33, 16, 40];
	const result = ages.filter(checkAdult);

	function checkAdult(age) {
	  return age >= 18;
	}
	
### Find Method
- Find method returns the first element from the array that passes the test.
- It returns undefined if no element passes the test(function).
#### Example-
	const ages = [32, 33, 16, 40];
	const result = ages.find(checkAdult); //returns 32 only 

	function checkAdult(age) {
	  return age >= 18;
	}

### Reduce Method- 
- It returns only the single value, i.e, the calculated result from the function.
- It takes in an initial starting element as the argument.
- If initial value is not provided, then the first element of the array is assigned as initial element.
#### Example-
	const num = [1, 2, 4, 6];
	const result = num.reduce(add);

	function add(initial, current){ 
	    return initial + current;  // takes initial element as num[0], i.e, 1
	}
	
### Sort Method-
- Sorts the elements of the array.
#### Example-
	const fruits = ["Banana", "Orange", "Apple", "Mango"];
	fruits.sort((a,b) => {
     if(a < b) return -1;
     if(a > b) return 1;
     return 0;
     }));  // returns ["Apple", "Banana", "Mango", "Orange"]

### References-
- https://www.w3schools.com/js/js_array_methods.asp
- https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array

