# Snippetstudy_primitives-types

## Description
This is about studying the primitive data types, how operators work and type conversions. Here, we talk about States and Operation. the operation does something, and the console returns a state. and so on.

<!---
personal note: use ctrl+f and lookup "continued" to find where you haven't finish.
-->

## Learning objectives (keywords)
* Primitive data types (type, value)
* Type conversions
* Operators

## Code snippet #1
```js
typeof (typeof Number(void Boolean(null))).toString();
    // s0: (Null, null)
    Boolean(null);
    // s1: (Boolean, false)
    void false;
    // s2: (Undefined, undefined)
    Number(undefined);
    // s3: (Number, NaN)
    (typeof NaN);
    // s4: (String, "number")
    ("number").toString();
    // s5: (String, "number")
    typeof "number";
    // s6: (String, "string")
```
[repl.it](https://repl.it/@colevandersWands/primitive-types)  
[PythonTutor](https://goo.gl/QahvNv)  
[Debugger](https://www.w3schools.com/code/tryit.asp?filename=FU1BIF6VJMS4) 
   
S0. (State 0) you begin with the starting point: null   
S1. _to be continued_
   
Tracing table (deconstruction of input/output):
   
State nr. | State | Operation
------------|------------ | -------------
S0  | null |  
 . |  | Boolean (null)
S1 | false | 
. | | Void (undefined; "undefined")
S2 | undefined | 
. |  | Number (Number; Nan)
S3 | Nan | 
. |  | typeof (string; "Number")
S4 | "Number" | 
. | | "Number".toString
S5| "Number" | 
. | | typeof "number" (BECAUSE "number" is actually a string. "n-u-m-b-e-r"
S6 | "string" | 

## Code Snippet #2
````js
var result;
var number = 10;

result = typeof Boolean (void (number.toString()) + String(null)).valueOf();

console.log(result);

````
[PythonTutor](http://www.pythontutor.com/javascript.html#code=var%20result%3B%0Avar%20number%20%3D%2010%3B%0A%0Aresult%20%3D%20typeof%20Boolean%20%28void%20%28number.toString%28%29%29%20%2B%20String%28null%29%29.valueOf%28%29%3B%0A%0Aconsole.log%28result%29%3B&curInstr=4&mode=display&origin=opt-frontend.js&py=js&rawInputLstJSON=%5B%5D)
[Repl.it](https://repl.it/@Joaoviana/CodeSnippet)
## Code Snippet #3
````js
var result;
var number = 10;

result = typeof Boolean (void (number.toString()) + String(null)).valueOf();
number.toString();
// s0 : (String, '10')
String(null);
// s0 : (String, 'null')
void('10');
// s1: (undefined, undefined)
(undefined+ 'null').valueOf();
// s2: (string, 'undefinednull')
Boolean ('undefinednull');
//s3: (Boolean, true)
typeof true;
//s4 (string, 'boolean')
````
S0. number.toString() converts number variable 10 to a string '10' ; String(null) converts it to string 'null'   
S1. void operator makes variable undefined - it acts as a 'dissociation' of its passed value   
S2. valueOf() returns the primitive value of a Number; however, it is taking 'undefinednull' string as an argument.   
S3. Boolean Primitive takes in a string and returns true.   
S4. typeof true is string 'Boolean'   
  
## Helpful Links

## Vocabulary

### Primitive data-types
Undefined: only one value, undefined  
Null: only one value, null   
Strings: anything between quotes. "anything"   
Number: [0-9], NaN (Not a Number), Inf (Infitnity)  
Boolean: True/False   

### Operators
JavaScript operators are used to assign values, compare values, perform arithmetic operations, and more.   
Typeof: it is a Type operator. Returns the type of variable. Takes anything mentionned before and makes it a string   
Void: takes everything and makes it undefined (not absolutely useful)   

### Misc
Repos: repository.   
Fork (Github): have an updated copy of a repository. can pull request to the OP, the OP can accept or refuse.   
Clone (Githbu): have a "static" copy of a repository. It is not linked in any ways to the OP repos.   

## Review
* Struggles: 
  * how the value "number", which is already a string, becomes "string" after the operator "typeof" is executed.
  * hoisting.
* Learning objectives that need extra work?   
  value, type
  difference between primitive type and operators
* next steps: 
  * 12345-345
  * strenghten my vocabulary
  
