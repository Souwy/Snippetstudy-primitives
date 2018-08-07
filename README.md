# Snippetstudy-primitives

## Description
This is about studying the primitive data types, how operators work and type conversions. Here, we talk about States and Operation. the operation does something, and the console returns a state. and so on.

<!---
personal note: use ctrl+f and lookup "continued" to find where you haven't finish.
-->

## Learning objectives (keywords)
* Primitive data types (type, value)
* Type conversions
* Operators

## Code snippet
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
[pytut](https://goo.gl/QahvNv)  
[debugger](https://www.w3schools.com/code/tryit.asp?filename=FU1BIF6VJMS4) 
   
S0. (State 0) you begin with the starting point: null   
S1. _to be continued_

## State & operation back-and-forth

state nr. | State | Operation
------------|------------ | -------------
S0  | null |  
S1  |  | Boolean (null)
S2 | false | 
S3 | | Void (undefined; "undefined")
S4 | undefined | 
S5 |  | Number (Number; Nan)
S6 | Nan | 
S7 |  | typeof (string; "Number")
S8 | "Number" | 
S9 | | "Number".toString
S10| "Number" | 
S11 | | typeof "number" (BECAUSE "number" is actually a string. "n-u-m-b-e-r"
S12 | "string" | 


## Helpful Links

## Vocabulary

### Primitive data-types
Undefined: only one value, undefined  
Null: only one value, null   
Strings: anything between quotes. "anything"   
Number: [0-9], NaN (Not a Number), Inf (Infitnity)  
Boolean: True/False   

### Operators
JavaScript operators are used to assign values, compare values, perform arithmetic operations, and more. You have
Typeof: it is a Type operator. Returns the type of variable. Takes anything mentionned before and makes it a string   
Void: takes everything and makes it undefined (not absolutely useful)   

### Misc
repos: repository.   
fork (Github): have an updated copy of a repository. can pull request to the OP, the OP can accept or refuse.   
clone (Githbu): have a "static" copy of a repository. It is not linked in any ways to the OP repos.   

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
  
