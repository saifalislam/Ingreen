# Ingreen
console.log('Hello world!')
console.error('This is the error')
console.warn('this is the last warning')
// variable 
let score;
score = 400;
const value=50;
console.log(value)
console.log(score)
// string, Numbers, Boolean, null, undefined, symbol
const name = 'Saif';
const x = null;
const age = 28;
const decimalnumber = 4.5;
const isCool = true ;
console.log(typeof score);
console.log(typeof age);
console.log(typeof isCool);
console.log(typeof name);
console.log(typeof x);
console.log(typeof value)
// Concatination 
console.log('My name is '+ name +' and i am '+age+' years old')
// Template string 
console.log('My name is ${name} and i am $ {age}');
// template string is not workig 
console.log(name.length); 

const s = 'How is it going';
console.log(s.toUpperCase());
console.log(s.toLowerCase())
console.log(s.substring(0,6).toUpperCase());
console.log(s.split(''));
console.log(name.split(''))
// Arrays - basically variable that hold multiple values
const number = new Array (1,2,2,4,5,5,8);
console.log(number);
const fruits = ['apples', 'oranges', 'pears', 10, true];
// In Java Script you can have multiple data types within the an array, 
// JS gives lot of Freedoms 
// JS is not staticly typed

console.log(fruits);
console.log(fruits[1]);
// in JS you can add values to the arry like followed below
fruits[5] = 'banans';
fruits.push('mangos');
fruits.unshift('50');
console.log(fruits);
fruits.pop(); // deleting an Array 
console.log(fruits);
// for checking anything need to put into conditional
console.log(fruits.indexOf('banans'))
console.log(Array.isArray(fruits));
// There are bunch of other methods to learn 
// Now time to learn Objects Literals
const person = {
    firstName: 'Saif',
    lastName: 'Al Islam',
    age: 25,
    address: {
        street: ['Gabtoli','bus stand'],
        HouseNumber: 52, 
        City: 'Narsingdi',
    },
    education: {
        NameofSchool: 'JQKM', 
        NameofCollege: 'NMC',
    }
}
console.log(person.education);
console.log(person.address.street[1]);
const { firstName, lastName, address: { city }} = person;
console.log(firstName);
console.log(city); // Could not find what is the problem
 // arrays of todos 
 const todos = [
     {
         id: 1, // Do not understand why i can not use a, b, c or as id . 
         text: 'My work format', 
         isCompleted: true
     },
     {
         id: 2,
         text: 'My school work',
         isCompleted: true
     },
     {
         id: 3,
         text: 'My home work ',
         isCompleted: false
     }
 ]
 console.log(todos[2].text);
/**Need to know little bit about JASON. 
 * Jason is a data format and its used a 
 * lot within full stack development 
 * and API when sending data to a server, usually send 
 * it in JASON format and receive it in JASON format.
 *  very simmiler to Object literals
 */
const todoJSON = JSON.stringify(todos);
console.log(todoJSON);
// For loops 
// while loops 

// for loops 
for (let i = 0; i <= 10; i++) {
    console.log(i); 
    // object literals 
    console.log ('for loop number: $(i)');
}
// while loops
let i = 0;
while(i<10) {
    console.log(i); 
    i++; 
}
 // looping through an Array 
for (let i = 0; i < todos.length; i++) {
    console.log(todos[i].text); 
} // another way of looping through is (for of loop)
for (let todo of todos){
    console.log (todo.text);
    console.log(todo.id);
}
// High order Array methods like foEach, map, filter
todos.forEach (function(t){
console.log(t.text)}
)
const tada= todos.map(function (t) {
    return t.id;
});
console.log (tada);
const tede = todos.filter (function (t)
{
    return t.isCompleted === true;
}).map(function(t)
 { return t.text}
)
console.log(tede);
// conditional
const X =10;
if (X==10){
    console.log('x is 10');
} else if (X > 10){
    console.log( 'X is greater than 10');
} else ('X is equal of smaller than 10');
