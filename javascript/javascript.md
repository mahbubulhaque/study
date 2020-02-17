# Javascript
**git repo for V8 Javascript engine :**
https://github.com/v8/v8
https://v8.dev/docs
## Coercion : 
**article link :** 
https://www.freecodecamp.org/news/js-type-coercion-explained-27ba3d9a2839/
http://www.adequatelygood.com/Object-to-Primitive-Conversions-in-JavaScript.html


**Definition:** 
Type coercion is the process of converting value from one type to another (such as string to number, object to boolean, and so on). Any type, be it primitive or an object, is a valid subject for type coercion.

There are two types of coercion. 
* implicit coercion
* explicit coercion

***Explicit coercion:***
When a developer expresses the intention to convert between types by writing the appropriate code, ``Number(value)`` it’s called explicit type coercion (or type casting).

***Implicit coercion:***
Since JavaScript is a weakly-typed language, values can also be converted between different types automatically, and it is called implicit type coercion. example: 
``1 == null``,  ``6/'2'``,  ``null + new Date()`` etc.

**example exercise to test myself :**
```
true + false
12 / "6"
"number" + 15 + 3
15 + 3 + "number"
[1] > null
"foo" + + "bar"
'true' == true
false == 'false'
null == ''
!!"false" == !!"true"
[‘x’] == ‘x’
[] + null + 1
[1,2,3] == [1,2,3]
{}+[]+{}+[1]
!+[]+[]+![]
new Date(0) - 0
new Date(0) + 0
{} + {}
a = 012
```
for more fun check wtfjs.com
### Concept:
The first rule to know is there are only three types of conversion in JavaScript:
* to string
* to boolean
* to number

Secondly, conversion logic for primitives and objects works differently, but both primitives and objects can only be converted in those three ways.