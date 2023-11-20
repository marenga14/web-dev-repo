## GET STARTED WITH JS

### WITH KYLE SIMPSON

### THREE PILLARS OF JS

i) Types and coersion
ii) scope and closure
iii) this/Prototypes

### INTRODUCTION

#### PROGRAMMING PRIMER IN JS

a) Value

-> 42 and 3.14 in js there's no distinction between the decimal and non-decimal number they're all number
-> "Hello world " this we call them strings

-> true & false , boolean

-> null & undefinied this we call them empty values, we have two of them,
-> arrays, and key value demostrations

- b) Operations

  -> Arithmetic such as 43 +3, this is addition incase of numbers
  -> "name " + "name2", this means this are the string concatibation
  Depends on the operands they determine what plus does this we call it OVERLOADING

  -> The plus and whatever that invlolve two oprrands its called the binary operandors, but the !false this is called the unary operator since it invloves only one operandor

c) Typeof
-> Typof `[1,2,3]` ,returns the "object" as the subtype of an object type

d) Variables
is the symblic representation of some place where our value are going to be stored, eg
var name = "Julius Marenga ", take the value and stores it in the variable name.

e) Expression and statement

var age = 23; this is the statement, and the = 23 is an expression (assignment expression )

f) if & Else statement

g) Loop

This we call it an iterator to some sort
for (student of students ){

}

h) functions
speaking of the interpolated mark, sort of the interpolated string
-> function could take a vaalue and do computation
-> function that returns the value back, with the return keyword

g)

### TYPES AND COERSION

a) Primitive types

-> not true that everything is like an object

. undefined
. string
. boolean
. object
. number
. symbol

`In javascript we are not talking about the types of varables but the type of the value, the typeof undefined (don't exists) varable is "undefined"`

-> `typeof null` gives the `"object"`, named as the historical bug of js.

- NaN, not a number

`var greeting = "hello class"
var something = greeting/2`
`something beclomes NaN`

`Number.isNaN (something ) // true
Number.isNaN (grreting ) //fasle`

b) Converting types (Type coersion )

-> New keyword for instatiaate the new isntances of object, we don't use the string, mumber,boolean etc rather we use them as the function.

-> Plus operator is oveloaded, to perform the implicit coersion , where the number + string = string

crazzy!!!!! all value properties from the dom are strings, so getting the number wwant to use it we need to coerse it to the number for it to work

-> Boolean
`
Falsy and Truthy
0 "foo"
null "everything else becomes true"
NaN
false
undefined
empty string`

-> Coersion and Best Practices

c) Checking Equality
check the values using the double equal and tripple equal, what does this mean ?

Double equal allows coersion when the types are'nt the same and the tripple equals doesnt allow coersion.

The point is the if we make the type so obvious, then double equal and tripple equal are technically the same thing.

-> `Javascript is dynamically typed language and we could embrace that, including the types and stuffs.`

### SCOPES AND CLOSURES

Rules of scope, if the varable isnt't defined in the function the variable will be found on the outa scope.

if non-strict the variable is undeclared it be created in the global scope.

UNDEFINED & UNDECLARED VALUES
Undefined and undecalared are basically reffered as the same thing most of the time only distinctly different.

FUNCTIONS EXPRESSIONS

Is the function as the values assigned some where, then function is the first class value.
example
`var clickWhat = functon ()`
`{}`
-> this is annonymous function expression

`var clicWhat = function hand (){}, this is reffered to as the named function expression`

**\* More on name && Unamed function expression **

`IIFES`
immediately invoked function expression
`var teacher = "kyle"
(
function anotherTecaher () {
var teacher = "suxxy "
}
) ()`

//helps to enapsulate the scope , like if we print the teacher out there the "kyle " // //will //
be maintained

#### PERFORM BLOCK SCOPING WITH LET KEYWORD

We use the let keyword so as to protect the varable from the global level modification of variables ,

`` function blockLevel (){
let name; // name is the functional level variable\

`` {
let blockEl;

//this isdefined only to this block, hence block level element and not in the whole function.

} ``

}``

#### CLOSURE AFTER UNDERSTANDING SCOPE

-> The function that remembers the variables outside of it, even if the function is passed else where.

-> it happens when we pass that function as the value somewhre else, like callback or anything like that .

### THIS && PROTOTYPE SYSTEM

this key word, references the execution context for that call, determine entirely by how the function was called .

Explicit binding -> one function to be reused in different places.

PROTOTYPES
What does prototype means?

prototype is an object of any instances are going to be linked to or to delegate to,
