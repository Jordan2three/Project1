# Project1/notes
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


// Concept - Loops

vacationSpots = ['QLD', 'NSW', 'SA'];
console.log(vacationSpots[0]);
console.log(vacationSpots[1]);
console.log(vacationSpots[2]);
// a tedious task without implementing loops

// Loops are used to repeat a set of instructions or block of code

// iterator variable; stopping condition; iterator statement

/* iterator variable is given it's value, the stopping condition (boolean) is evaluated against the iterator variable, the iterator statement is updated against the iterator variable on each loop
*/

//For example

for(let counter = 5; counter < 11; counter++) {
  console.log(counter);
}
/* Output
    5
    6
    7
    8
    9
    10
*/


for (let counter = 3; counter >= 0; counter--){
  console.log(counter);
}


/* for is the command that initialise a loop
let is the declaration of the variable
counter is the variable name, in this case the counter is assigned (=) the integer 3. This section of the code in a loop is known as the iterator variable.

The next set of texts is the Stopping Conditions. Here we see that this results in a boolean value. The counter variable is using a comparison operator >= (more than or equal to) to the value 0

The last set of text is known as the iterator statement. counter-- uses the variable counter then decreases it's value by 1.

Overall the variable counter is assigned the value 3. Then counter is checked to see if it's value is greater than or equal to 0. In this case, the boolean is true. So now the iterator statement executes, which now changes the value of 3 to now 2.
Because this is initialised with the  for  operator, it automatically loops the code until the boolean value becomes false, then ceases to operate.
*/

const vacationSpots = ['Bali', 'Paris', 'Tulum'];
for (let i = 0; // Create a variable and assign it a value

i < vacationSpots.length; // Create a boolean expression. You ideally want this to be true, then loop until it becomes false

i++) // What do you want your code to repeat until the boolean value becomes false

{
  console.log(`I would love to visit ${vacationSpots[i]}`) // What you are printing to the console, and use interpolation to have access to the arrays in the previous code
  // Here we are using interpolation to insert vacationSpots (Bali, Paris, Tulum) but also referencing it's index values to loop the text but ends at each index. Then creates a new line of text with the same string but referencing another index.
}

// A Loop running inside a loop is known as a nested loop. Nested loops are generally used to compare the elements in two arrays.
// For each round of the outer  for  loop, the inner  for  loop will run completely.
// Example
const myArray = [6, 19, 20];
const yourArray = [19, 81, 2];
for (let i = 0; i < myArray.length; i++) {
  for (let j = 0; j < yourArray.length; j++) {
    if (myArray[i] === yourArray[j]) {
      console.log('Both arrays have the number: ' + yourArray[j]);
    }
  }
}

const bobsFollowers = [ 'Jake', 'Amber', 'Zack', 'Tim' ];
const tinasFollowers = [ 'Chloe', 'Jake', 'Zack' ];
const mutualFollowers = [];

for (let i = 0; i < bobsFollowers.length; i++ ) {
  for (let j = 0; j < tinasFollowers.length; j++) {
    if (bobsFollowers[i] === tinasFollowers[j]) {mutualFollowers.push(bobsFollowers[i]);
    }
  }
}

console.log(mutualFollowers) //prints [ 'Jake', 'Zack']



// while loops

const cards = ['diamond', 'spade', 'heart', 'club'];


let currentCard = 'heart'
while (currentCard !== 'spade') {
  currentCard = cards[Math.floor(Math.random() * 4)];
  console.log(currentCard)
}

// do while statements

let cupsOfSugarNeeded = 3
let cupsAdded = 0

do {
  cupsAdded++
 console.log(cupsAdded + ' cups were added') 
}
  while (cupsAdded < cupsOfSugarNeeded);


// break keyword

const rapperArray = ["Lil' Kim", "Jay-Z", "Notorious B.I.G.", "Tupac"];

for (let i = 0; i < rapperArray.length; i++) {
  console.log(rapperArray[i])
if (rapperArray[i] === 'Notorious B.I.G.') {
  break
  }
}
console.log("And if you don't know, now you know.")




let userName = 'Jane';
let userQuestion = 'Is it going to rain today?';
let randomNumber = Math.floor(Math.random() * 9);
let eightBall = ''


userName ? console.log(`Hello, ${userName}!`): console.log('Hello!'); 

console.log(`${userQuestion}`);
console.log(`${randomNumber}`)

switch (randomNumber) {
  case 0:
  eightBall = 'It is certain'
  break;

  case 1:
  eightBall = 'It is decidedly so'
  break;

  case 2:
  eightBall = 'Reply hazy try again'
  break;

  case 3:
  eightBall = 'Cannot predict now'
  break;

  case 4:
  eightBall = 'Do not count on it'
  break;

  case 5:
  eightBall = 'My sources say no'
  break;

  case 6:
  eightBall = 'Outlook not so good'
  break;

  case 7:
  eightBall = 'Who knows, really'

default:
eightBall = 'Signs point to yes'

}

console.log(`The magic eightball says "${eightBall}"`)
