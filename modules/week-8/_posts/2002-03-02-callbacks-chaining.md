---
title: Callbacks and Chaining
module: 8
jotted: false
---


# Callbacks and Chaining

<div class="tab">
  <button class="tablinks active" onclick="openTab(event, 'Overview')">Overview</button>
<button class="tablinks" onclick="openTab(event, 'callbacks')">Callbacks</button>
<button class="tablinks" onclick="openTab(event, 'chaining')">Chaining</button>

</div>
<div id="Overview" class="tabcontent" style="display:block">
<div class="tabhtml" markdown="1">

What are these?  These extend our jQuery functionality even more.  They are really helpful and will reduce code required to accomplish the same task.

</div>
</div>

<div id="callbacks" class="tabcontent">
<div class="tabhtml" markdown="1">

## Callbacks

With each jQuery method, you can also add a callback function.  What is that?  A callback function is a function that is  called when the first function has completed.  Let's look at an example.

```html
<!DOCTYPE html>
<html>

<head>
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.3.1/jquery.min.js"></script>
    <script>
        $(function () {


        });
        $(document).ready(function () {
            $("button").click(function () {
                 $(".myGreatClass").fadeOut("slow", function(){
                     $("#infoid").toggle();
                 });
            });
        });
    </script>
</head>

<body>

    <p id="infoid">This is a paragraph.</p>
    <p class="myGreatClass" style="background-color:red">This is the second paragraph.</p>
    <button>Click me to hide paragraphs</button>
    <br>
</body>

</html>
```

So, what just happened?  The paragraph element fades out slowly when the button is clicked.  After the paragraph fades away, then the paragraph with the id **infoid** will toggle.  Keep in mind, it doesn't have to be another jQuery method, it can anything you want in there.

<div class="embed-responsive embed-responsive-16by9"><iframe class="embed-responsive-item" src="https://www.youtube.com/embed/YfoY3_36cHM" frameborder="0" allowfullscreen></iframe></div>


</div>
</div>

<div id="chaining" class="tabcontent">
<div class="tabhtml" markdown="1">

## Chaining

So, what is chaining?  This allows us to call multiple methods and have them apply to the same element.  One example might look like this:

```html
<!DOCTYPE html>
<html>

<head>
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.3.1/jquery.min.js"></script>
    <script>
        $(function () {


        });
        $(document).ready(function () {
            $("button").click(function () {
                 $(".myGreatClass").fadeOut("slow").fadeIn("slow");
            });
        });
    </script>
</head>

<body>

    <p id="infoid">This is a paragraph.</p>
    <p class="myGreatClass" style="background-color:red">This is the second paragraph.</p>
    <button>Click me to hide paragraphs</button>
    <br>
</body>

</html>
```

Using the dot operator, we can chain multiple jQuery functions together and have them execute one after another.  Cool huh?

<div class="embed-responsive embed-responsive-16by9"><iframe class="embed-responsive-item" src="https://www.youtube.com/embed/w-2W1CS8mbg" frameborder="0" allowfullscreen></iframe></div>

</div>
</div>

