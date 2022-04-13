Welp, making a snowman was rough. But now I'm gonna make it all better... with colors!

The only colors we have used so far are... well default colors. And like anything thats the default... they're always boring.

# Background Color
We'll start with the simplest color... the background! The following program makes a screen of 400 x 400, and sets the background color to black.

```java
size(400, 400);

background(0, 0, 0);
```

If you are a diehard programmer you can skip this explanation and head strait to the docs here [https://processing.org/reference/#color](https://processing.org/reference/#color)

Otherwise keep reading for my exemplary guidance.

If you run this code, you won't see anything exciting. Just a black void. Lets draw a rectangle on top of the void (and hopefully make it less void'ish).

(here is my code)
```java
size(400, 400);

background(0, 0, 0);

rect(0, 200, 100, 100);
```

If you run the above code you should see a square on a black background!

![black void square processing.js processing spark3d](/Assets/black-void-square.png)

Yay!

If you put the `rect` command *before* the background command...

```java
size(400, 400);

rect(0, 200, 100, 100);

background(0, 0, 0);
```

...then the background will be drawn on top of the square (hence you won't see the rectangle).

![black void processing.js processing spark3d](/Assets/black-void.png)

This is important... the order we put commands in, is the order that they will get "painted" onto the screen.

So, make sure to draw your shapes *after* you draw the background! Otherwise the background will get painted on top of the square. Painting the background on top of shapes is also how you can "clear" the screen to be a solid color. This will be useful later in section 04 - Variables.

![black void square processing.js processing spark3d](/Assets/black-void-square.png)

# Colors?
So how do these colors work? Why did we get black when we put `(0, 0, 0)`?

The numbers are for amounts of Red Green and Blue.

RGB Colors!

Each number can range from 0 to 255 (255 is the max!). Now with this knowledge, lets color some shapes!

# Coloring Shapes
Ironically, the command for "filling" in the color of shapes is `fill`.

```java
size(400, 400);

background(0, 0, 0);

fill(255, 0, 0);

rect(0, 200, 100, 100);
```

Any shapes after our fill command will now be red!

![](/Assets/fill-red-square.png)

Go ahead and add a few more shapes!

![](/Assets/fill-red-squares.png)

And here is the code I used.

```java
size(400, 400);

background(0, 0, 0);

fill(255, 0, 0);

rect(0, 200, 100, 100);

rect(40, 10, 100, 100);

rect(200, 200, 50, 60);
```

There is a bit of a problem here though! How do I get different colors? Well, its pretty easy, just put a `fill` comand before the shape(s) you want to change the color of!

Lets put a `fill` command right before the last `rect` command. I will set the color to be blue (feel free to pick a different color).

```java
size(400, 400);

background(0, 0, 0);

fill(255, 0, 0);

rect(0, 200, 100, 100);

rect(40, 10, 100, 100);

// blue
fill(0, 0, 255);

rect(200, 200, 50, 60);
```

If you add a `fill(0, 0, 255);` command right before the last shape you should see the last rectangle be colored blue!

![fill-cubes-colors](/Assets/fill-cubes-colors.png)

TADA! Now lets make an Owl with this in the next section!