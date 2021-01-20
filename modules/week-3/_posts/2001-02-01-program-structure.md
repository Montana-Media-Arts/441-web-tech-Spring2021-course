---
title: Program Structure
module: 3
jotted: true
---

# Program Structure

<div class="tab">
  <button class="tablinks active" onclick="openTab(event, 'Overview')">Overview</button>
  <button class="tablinks" onclick="openTab(event, 'Bindings')">Bindings</button>
  <button class="tablinks" onclick="openTab(event, 'Functions')">Functions</button>
  <button class="tablinks" onclick="openTab(event, 'Controls')">Controls</button>
  <button class="tablinks" onclick="openTab(event, 'Assignments')">Assignments</button>
  <button class="tablinks" onclick="openTab(event, 'ToDo')">To Do</button>
</div>
<div id="Overview" class="tabcontent" style="display:block"  markdown="1">
Consider reading the following

- Haverbeke, Marijn. **Eloquent JavaScript: A Modern Introduction to Programming.** 3rd Edition. N.p., 2018. Web.
    - [_Chapter 2; Program Structure_](http://eloquentjavascript.net/3rd_edition/02_program_structure.html)
- **JavaScript Guide.** MDN web docs. 2018. Web.
    - [_Control flow and error handling_](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Control_flow_and_error_handling)
    - [Loops and Iteration_](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Loops_and_iteration)

</div>

<div id="Bindings" class="tabcontent">
<div class="tabhtml" markdown="1">

- _Bindings_
    - `let`
    - `var`
    - `const`
        - Recognize that the latter of these is unchangeable

#### Using let and const (2015)

Before 2015, using the **var** keyword was the only way to declare a JavaScript variable.

The 2015 version of JavaScript (ES6 - ECMAScript 2015) allows the use of the **const** keyword to define a variable that cannot be reassigned, and the **let** keyword to define a variable with restricted scope.

#### Scope 
let and const two keywords provide **Block Scope** variables (and constants) in JavaScript.

Before ES2015, JavaScript had only two types of scope: Global Scope and Function Scope. 

**Global Scope**

Variables declared Globally (outside any function) have Global Scope.

```js
var carName = "Volvo";

// code here can use carName

function myFunction() {
  // code here can also use carName
}
```

**Function Scope**

Variables declared Locally (inside a function) have Function Scope.

```js
// code here can NOT use carName

function myFunction() {
  var carName = "Volvo";
  // code here CAN use carName
}

// code here can NOT use carName
```

**JavaScript Block Scope**

Variables declared with the var keyword cannot have Block Scope.

Variables declared inside a block {} can be accessed from outside the block.

```js
{
  var x = 2;
}
// x CAN be used here
```

Before ES2015 JavaScript did not have Block Scope.

Variables declared with the let keyword can have Block Scope.

Variables declared inside a block {} cannot be accessed from outside the block:

```js
{
  let x = 2;
}
// x can NOT be used here
```

**Video**
<div class="embed-responsive embed-responsive-16by9"><iframe width="560" height="315" src="https://www.youtube.com/embed/7OLJsDclVXY" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></div>
</div>
</div>
<div id="Functions" class="tabcontent">
<div class="tabhtml" markdown="1">
- Have a basic grasp of what a _Function_ is
    - especially;
        - `console.log()`
        - `prompt()`

**Video**
<div class="embed-responsive embed-responsive-16by9"><iframe width="560" height="315" src="https://www.youtube.com/embed/smVWNLrZnz4" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></div>
</div>
</div>
<div id="Controls" class="tabcontent">
<div class="tabhtml" markdown="1">
- Recognize that the _functions_ can produce _Return Values_
- _Control Flow_
    - As well as using _conditional execution_ with control flow
    - Understand how to use;
        - `if(){}`
        - `if(){} / else{}`
        - `if(){} / else if(){} / else{}`
        - `while(){}`
        - `do{}while()`
        - `break`
        - `switch`

**Video**
<div class="embed-responsive embed-responsive-16by9"><iframe width="560" height="315" src="https://www.youtube.com/embed/-UZdpIUFGQo" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></div>
</div>
</div>
<div id="Assignments" class="tabcontent">
<div class="tabhtml" markdown="1">
- Basic coding standards and conventions
    - Use proper "naming conventions" when creating bindings
        - Including what characters can and cannot be used
        - Utilize a single approach to capitalization
    - Indent Code Properly
    - Understand how to include comments
- assignment operators
    - `+=`
    - `-=`
    - `*=`
    - `/=`
    - `++`
    - `--`

**Video**
<div class="embed-responsive embed-responsive-16by9"><iframe width="560" height="315" src="https://www.youtube.com/embed/G4v2oGLIIYw" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></div>
</div>
</div>
<div id="ToDo" class="tabcontent" >
<div class="tabhtml" markdown="1">
## Interactive JS Console

Feel free to try out some of the prior examples.

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

<em><a href="https://www.w3schools.com/js/default.asp" target="_new">Reference</a></em>