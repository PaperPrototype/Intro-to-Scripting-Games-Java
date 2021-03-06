By the end of this lecture you will be able to make a snowman! And anything else you want to make :)

![processing-snowman](/Assets/processing-snowman.png)

# Drawing shapes
Start by writing this code.

```java
size(400, 400);

ellipse(100, 100, 100, 100);
```

Now click the play button!

![](/Assets/first-sketch.png)

Tada!

How did that work? We just told the computer to set the size of the window to 400 pixels by 400 pixels...

```java
size(400, 400);
```

And then on line 3 we drew an ellipse...

```java
ellipse(100, 100, 100, 100);
```

"ellipse" stands for an oval or circle.

`size` and `ellipse` are commands.

Now what about all the numbers in the parenthesis `(100, 100, 100, 100)`? Those are x and y positions on the screen.

X and Y start in the top left corner ands move out. Just like a graph in geometry!

![processing axis](/Assets/processing-axis.png)

The first 2 numbers in `ellipse` comand are for the top left position of the circle.

![](/Assets/ellipse-top-left.png)

And the second 2 numbers are for the width and height of the circle.

![](/Assets/ellipse-bottom-right.png)

You might notice that fact we have to put parenthesis `()` and commas `,` after `ellipse`.

Imagine if java didn't require them! The code would then look like this...

```java
ellipse100100100100
```

And, well, that is just hard to read. So we add parenthesis and comma's...

```java
ellipse(100, 100, 100, 100)
```

One last thing you might notice is that you have to put a semicolon `;` at the end of each command.

![](/Assets/semicolon.png)

That annoying little thing has to be there so java can tell lines of code apart. 

In a file the whole idea of a "newline" is often represented as this special `\n` character. So our code actually looks like this in the file under the hood.

```
\nsize(400, 400);\n\n\nellipse(100, 100, 100, 100);
```
Notice the `\n` in there? Yup, well things like google docs and, basically anything that deals with text, won't show you the newline character `\n`, they just make a newline so you see the following.

```java
size(400, 400);

ellipse(100, 100, 100, 100);
```

Anyhow, thats why we have semicolons at the end of each line of code!

# Challenge time!
Since drawing a single circle is pretty boring I'll tell you about the other shapes you can draw, then your job is to take those and make a snowman!

Here are the commands for other shapes (replace `x` and `y` with actual positions, same for any other words I shove in there liek `width` and `height`).

(circle [https://processing.org/reference/circle_.html](https://processing.org/reference/circle_.html))
```java
circle(x, y, extent);
```

`extent` equals the `width` and `height` of the circle.

(rect [https://processing.org/reference/rect_.html](https://processing.org/reference/rect_.html))
```
rect(x, y, width, height);
```

(line [https://processing.org/reference/line_.html](https://processing.org/reference/line_.html))
```java
line(x1, y1, x2, y2);
```

`x1` and `y1` are the position of one end of the line, and `x2` and `y2` are the position for the other end of the line.

You can view the longer list of commands here [here](https://processing.org/reference/#shape), but these should be enough for now.

Now take these shapes and build a snowman with some landscape! For reference here is my snowman :)

![processing-snowman](/Assets/processing-snowman.png)

And once your done you can save your code uisng `ctrl` + `s` (on mac it's `cmd` + `s`).

Or if your not a shortuct keys person, you can use the menu and do `File` then `Save`.