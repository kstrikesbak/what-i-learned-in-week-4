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

This was a great exercise to get us used to the if/else logic. 
The code block for 'if' will execute based the specified condition is true. If that condition is false, it will work downwards and see if is true against the 'if else'. If none of these are true, then else will be executed.  

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

## `TERNARY OPERATORS`

Different way of writing if/else statements. Takes in three arguments
1. comparison argument e.g. temp>=80
2. result if true
3. result if false 

```javascript
function isHot(temp) {
  return (temp>=80) ? 'Yes, it is indeed hot.' : 'No, it is not hot.'
  }


function helloThere(str) {
  return (str.length<=5) ? 'Hello' + ', ' + str : 'Hi' + ', ' + str ;
}


function goodbyeYou(str) {
  return (str===undefined) ? 'Goodbye, stranger' : 'Goodbye, ' + str;
}
```