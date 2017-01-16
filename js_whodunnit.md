#JS Day 1 Homework

Go through each sample code and work out what the output will be and explain what happened.

### Episode 1
```js
var name = 'Keith';

var printName = function() {
  console.log('My name is ' + name );
};

printName();

ANSWER: My name is Keith

### Episode 2
```js
score = 5;

var result = function() {
  var score = 3;
  return score;
};

console.log(result());

ANSWER: 3

### Episode 3
```js
var myAnimals = ['Chickens', 'Cats', 'Rabbits'];

var listAnimals = function() {
  myAnimals = ['Ducks', 'Dogs', 'Lions'];
  for(var i=0;i<myAnimals.length; i++){
    console.log(i + ": " + myAnimals[i]);
  }
}

listAnimals();

ANSWER:
  1: Ducks
  2: Dogs
  3: Lions

### Episode 4

```js
var suspectOne = 'Jay';
var suspectTwo = 'Val';
var suspectThree = 'Keith';
var suspectFour = 'Rick';

var allSuspects = function() {
  var suspectThree = 'Harvey'
  console.log('Suspects include: ' + suspectOne + ', ' + suspectTwo + ', ' + suspectThree + ', ' + suspectFour)
};

allSuspects();
console.log( 'Suspect three is:' + suspectThree );

ANSWER:
  Suspects include: Jay, Val, Harvey, Rick
  Suspect three is: Keith

### Episode 5

```js
var detective = {
  name : 'Ace Ventura',
  pet : 'monkey'
};

var printName = function(detective) {
  return detective.name
};

var detectiveInfo = function() {
  detective['name'] = 'Poirot'
  return printName(detective);
};

console.log(detectiveInfo());

ANSWER: Poirot

### Episode 6
```js
var murderer = 'rick';

var outerFunction = function() {
  var murderer = 'marc';

  var innerFunction = function() {
    murderer = 'valerie';
  }

  innerFunction();
}

outerFunction();
console.log('the murderer is ', murderer);
```
ANSWER: valerie

### Episode 7 - Make up your own episode/s!

Make up your own episode which can be whatever you wish and the rest of the class will work out together what happened and what the output will be.


var killer = 'Tegan'
var weapon = 'Dagger'
var place = 'CodeClan'

var others = []
var motives = function() {
  others.push("Will");
  others.push("Adam");
  others.push("Lewis");
  others.push("Ben");
  others.push(killer);
  console.log(others);
}

var investigate = function() {
var killer = "Winnie"
  motives();
  others.sort();
  var murderer = others[others.length - 1];
  console.log(murderer, "murdered", others[0], "with a ", weapon, "at", place);
}

investigate();







