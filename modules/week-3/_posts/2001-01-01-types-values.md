---
title: Types & Values
module: 3
jotted: true
---

# Values, Data Types, & Operators


<div class="tab">
  <button class="tablinks active" onclick="openTab(event, 'Overview')">Overview</button>
  <button class="tablinks" onclick="openTab(event, 'Operators')">Math Operators</button>
  <button class="tablinks" onclick="openTab(event, 'String')">String Operators</button>
  <button class="tablinks" onclick="openTab(event, 'Unary')">Unary Operators</button>
  <button class="tablinks" onclick="openTab(event, 'Comparison')">Comparison Operator</button>
  <button class="tablinks" onclick="openTab(event, 'ToDo')">To Do</button>
</div>
<div id="Overview" class="tabcontent" style="display:block"  markdown="1">
Consider reading the following

- Haverbeke, Marijn. **Eloquent JavaScript: A Modern Introduction to Programming.** 3rd Edition. N.p., 2018. Web.
    - [_Chapter 1: Values, Types, and Operators_](http://eloquentjavascript.net/3rd_edition/01_values.html)
- **JavaScript Guide.** MDN web docs. 2018. Web.
    - [_Grammar and Types_](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Grammar_and_Types)
    - [_Expressions and operators_](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators)

- **Values**
    - Regular Values
    - Empty Values
        - `null`
        - `undefined`
- **Data Types**
    - Numbers
        - Regular Numbers
        - Special Numbers
    - Strings
        - regular strings (`"Hello World!"`, `'single quote string'`)
        - special characters (i.e., `\n`, `\t`)
        - template literal strings (``these use backticks and have special properties``)
    - Booleans

### The latest ECMAScript standard defines nine types:

Six Data Types that are primitives, checked by typeof operator:

* undefined : typeof instance === "undefined"
* Boolean : typeof instance === "boolean"
* Number : typeof instance === "number"
* String : typeof instance === "string"
* BigInt : typeof instance === "bigint"
* Symbol : typeof instance === "symbol"

#### Structural Types:

**Object** : typeof instance === "object". Special non-data but Structural type for any constructed object instance also used as data structures: new Object, new Array, new Map, new Set, new WeakMap, new WeakSet, new Date and almost everything made with new keyword;

**Function** : a non-data structure, though it also answers for typeof operator: typeof instance === "function". This is merely a special shorthand for Functions, though every Function constructor is derived from Object constructor.

#### Structural Root Primitive:

**null** : typeof instance === "object". Special primitive type having additional usage for its value: if object is not inherited, then null is shown;
Keep in mind the only valuable purpose of typeof operator usage is checking the Data Type. If we wish to check any Structural Type derived from Object it is pointless to use typeof for that, as we will always receive "object". The indeed proper way to check what sort of Object we are using is instanceof keyword. But even in that case there might be misconceptions.

As we can see the meaning of every primitive type is obvious except of undefined and null which are almost the same. This happens as the concept of Time is strictly connected with the purpose of algorithms. We can purport something that does not yet exist or does not exist anymore: undefined. But when we wish to be able to represent something that exists being empty, we have to invent another keyword. And that is what null stands for: the beginning of structural meaning.

**Video**

<div class="embed-responsive embed-responsive-16by9"><iframe width="560" height="315" src="https://www.youtube.com/embed/XSI_ta0mvOE" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></div>

</div>

<div id="Operators" class="tabcontent">
<div class="tabhtml" markdown="1">


**Mathematical Operators**
    
JavaScript Arithmetic Operators

Arithmetic operators perform arithmetic on numbers (literals or variables).

**Operator	    Description**
`+`	            Addition
`-`	            Subtraction
`*`	            Multiplication
`**`	        Exponentiation
`/`	            Division
`%`	            Modulus (Remainder)
`++`	        Increment
`--`	        Decrement

**Video**

<div class="embed-responsive embed-responsive-16by9"><iframe width="560" height="315" src="https://www.youtube.com/embed/isrkyyJfAz4" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></div>

</div>
</div>

<div id="String" class="tabcontent">
<div class="tabhtml" markdown="1">
    - String operators
        - String concatenation (`+`)
    
**Video**
<div class="embed-responsive embed-responsive-16by9"><iframe width="560" height="315" src="https://www.youtube.com/embed/DTk3ptbINGo" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></div>
</div>
</div>

<div id="Unary" class="tabcontent" >
<div class="tabhtml" markdown="1">
    - Unary Operators
        - `typeof`

    
**Video**
<div class="embed-responsive embed-responsive-16by9"><iframe width="560" height="315" src="https://www.youtube.com/embed/O6_MphRS0E8" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></div>
</div>
</div>

<div id="Comparison" class="tabcontent">
<div class="tabhtml" markdown="1">
    - Comparison Operators
        - `<`, `>`,`<=`, `>=`, `==`, `!=`
    - Logical Operators
        - or - `||`
        - and - `&&`
        - not - `!`
    - Type Conversion
    
**Video**
<div class="embed-responsive embed-responsive-16by9"><iframe width="560" height="315" src="https://www.youtube.com/embed/yjg6D7B7ozM" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></div>

</div>
</div>

<div id="ToDo" class="tabcontent" >
<div class="tabhtml" markdown="1">
## Interactive JS Console

While you work on this chapter, you should use the following interactive JS console to test out values, types, and operators.

<div id="jotted-demo-1" class="jotted-theme-stacked"></div>

<script>
    new Jotted(document.querySelector("#jotted-demo-1"), {
    files: [
        {
            type: "js",
            hide: false,
            content: "// try out operators, values, etc, here...\n\n// as an example\nconsole.log( typeof \"Hello World!\");\nconsole.log( 5*10 == 50 );\n\n\n"
        }
    ],
    showBlank: false,
    showResult: false,
    plugins: [
        { name: 'ace', options: { "maxLines": 50 } },
        { name: 'console', options: { autoClear: false } },
    ]
});
</script>
</div>
</div>
