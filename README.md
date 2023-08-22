# Project1
// Just started learning to code, using this project to practice and as a reference point


/* Using the concept of Arrays; create a list using the following information.

Task 1
New Years Resolution
  1. Keep a journal
  2. Take a falconry class
  3. Learn to juggle

  Task 2
Ranking Soda
  1. Coke Zero
  2. Dr. Pepper
  3. Sprite
*/

let newYearsResolution = ['Keep a journal', 'Take a falconry class', 'Learn to juggle'];

let sodaRanking = ['Coke Zero', ' Dr.Pepper', ' Sprite.'];

console.log(newYearsResolution);
// In the following exercise, I have used String Interpolation alongside with the concept of Arrays
console.log(`My favourite soda\'s are the following: ${sodaRanking}`);





// Concept - Array Index, Updating Arrays

// create an Array using the following indexes: Leaves, Branch, Root.

let tree = ['Leaves', 'Branch', 'Root'];
console.log(tree);
// now update Branch (by referencing it's index position) to 'Trunk'

tree[1] = 'Trunk';

// print the updated tree array so that it's now [ 'Leaves', 'Trunk', 'Root' ]

console.log(tree);




// Concept - re-assigning arrays

let condiments = ['Ketchup', 'Mustard', 'Soy Sauce', 'Sriracha'];

const utensils = ['Fork', 'Knife', 'Chopsticks', 'Spork'];

// re-assign the element in index 0 of condiments 'Ketchup' to 'Mayo'

condiments[0] = 'Mayo'; // 'Ketchup' now re-assigned to 'Mayo'
console.log(condiments); // prints [ 'Mayo', 'Mustard', Soy Sauce', 'Sriracha' ]

condiments = ['Mayo']; // array condiments now completely re-assigned to a single array

console.log(condiments); // prints [ 'Mayo' ]

utensils[3] = 'Spoon' // An element/index value in a const array can be reassigned so the outcome should print 'Spoon' instead of 'Spork'
console.log(utensils); // prints [ 'Fork', 'Knife', 'Chopsticks', 'Spoon' ]





// concept .length

// Use the .length property to the previous arrays (utensils, condiments, tree) to find it's element output

const objectives = ['Learn a new language', 'Read 52 books', 'Run a marathon'];
console.log(objectives.length); // Output: 3

console.log(utensils.length); // Output: 4
console.log(`Number of utensils is: ${utensils.length}`); // prints 'Number of utensils is: 4'

console.log(condiments.length); // Output: 1 . This is the most updated value/element for the array

console.log(`The updated number of condiments is now: ${condiments.length}`); // Output 'The updated number of condiments is now: 1'

console.log(tree.length); // Output: 3
console.log(`A tree has mainly ${tree.length} components`); // Output 'A tree has mainly 3 components


// Concept - .push()

const chores = ['wash dishes', 'do laundry', 'take out trash'];

// .push() is used to add additional elements to an existing array

chores.push('item 3', 'item 4'); // .push() here has added two additional elements to the array chores
console.log(chores); // prints [ 'wash dishes', 'do laundry', 'take out trash', 'item 3', 'item 4' ]
console.log(chores.length); // Output: 5



// Concept - .pop()


const groceryList = ['orange juice', 'bananas', 'coffee beans', 'brown rice', 'pasta', 'coconut oil', 'plantains'];

// Use the .shift() method to remove the first item of the groceryList array

groceryList.shift(); // 'orange juice' should now be removed from the array, and 'bananas' now shifted to be index 0 in the array
console.log(groceryList);

// Use the .unshift() method to add 'popcorn' to the beginning of the list

groceryList.unshift('popcorn'); // 'popcorn' should now be index 0 in the groceryList array, and 'bananas' is now index 1
console.log(groceryList);


// Use .slice() to provide a partial output of the array 'bananas', 'coffee beans', 'brown rice'
