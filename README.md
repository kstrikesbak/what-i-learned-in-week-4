# **WHAT I LEARNED IN  WEEK 4** 


## `FIZZY`
We worked in groups to code the `FIZZBUZZ` game. It was a great chance to collaborate and share ideas when coding this. It was also interesting to see other groups code. 

```javascript
function fizzy(num) {

if (num % 3 === 0 && !(num % 5===0)) {
    return 'Fizz';
} else if (num % 5 ===0 && !(num % 3===0)) {
  return 'Buzz';
} else if (num % 15 === 0) {
  return 'FizzBuzz';
} else {
    return num;
  }
}

console.log(fizzy(6));
```
___

## `Boolean Operators Exercise `

Write a function called moreThan5 that takes in a number and returns whether or not it's greater than 5.
Write a function called topScore that takes in a score (as a number) and a top score (as a number) and returns whether or not the score is greater than the top score. (This would be a good function in a game or gamified app to see if we need to update the high score).


```javascript
function moreThan5(num) {
  return num>5;
}

function topScore(score,top) {
  return score>top;
}

function isInDanger(grade) {
  return grade>= 60 && grade <=71;
}

function isCoasting(grade) {
  return grade>71 && grade<=83;
}

function isSucceeding(grade) {
  return grade>= 84 && grade <=92;
}

function isFailing(grade) {
  return grade<60;
}

function isAcing(grade) {
  return grade>92;
}

function isStudent(role) {
  return role === 'student';
}

function isTeacher(role) {
  return role === 'teacher';
}

function isAdmin(role) {
  return role === 'admin';
}

function isElementary(level) {
  return level === 'elementary';
}

function notAnElementarySchoolAdministrator(role,level) {
  return role !== 'elementary'|| level !== 'admin';
}

function isMiddleSchoolTeacher(role, level) {
  return role === 'teacher' && level>=6 && level<=8;
}

function differentPeople(name1,name2) {
  return name1 !== name2;
}
```
___

## `IF/ELSE EXERCISE`

Write a function called isItLong that returns the string 'That's a long string!' if the given string is longer than 20 characters. It should not return anything otherwise. (Explicitly, at least--every function returns undefined if you don't return a value!)

```javascript

function isItLong(str) {
  if (str.length>20) {
    return "That's a long string!";
  }
}

function isItMedium(str) {
  if (str.length >= 10 && str.length <= 20) {
    return "That's a regular sized string!";
  }

}

function isItShort(str) {
  if (str.length < 10) {
    return "That's a small string!";
  }

}

function howLongIsMyString(str) {
  if (str.length > 20) {
    return "That's a long string!";
  }
  else if (str.length >= 10 && str.length <= 20) {
    return "That's a regular sized string!";
  }
  else if (str.length < 10) {
    return "That's a small string!"; 
  }

}

function instructorHeight(str) {
  if (str === "Colin" || str === "colin") {
    return 62;
  }
  else if (str === "Mesuara" || str === "mesuara") {
    return 67;
  }
  else {
    return "I don't know that instructor!";
  }
}
```
