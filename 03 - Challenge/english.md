# Challenge Draw an Owl...?

By the end you will have an owl... chicken, thing.

![questionable owl](/Assets/questionable-owl.png)

Mr. Questionable Owl here is yur subject of art today.

First lets set the background and size of the window.

```java
size(400, 400);
background(5, 5, 100);
```

If you run this you will see a blue background!

![owl background](/Assets/owl-background.png)

# Comments
Once you start writing lots of code it will get hard to know what code does what. So we have comments (that the computer will ingore).

![owl setup comment](/Assets/owl-setup-comment.png)

Comments start with 2 slashes `//` and are ingored by the computer. It is very important to comment code! If I don't comment my code I often forget what that code does! 

# Head
Now make the owls head, and comment the code!
![owl head](/Assets/owl-head.png)

# Eyes
And now for the eyes!

![owl eyes](/Assets/owl-eyes.png)

I left some of the numbers as `0000`. Fill in all the `0000`'s with the correct number!

# Pupil Color
We want the pupils to be mostly dark. So we are going to use a fill color of `(1, 1, 5)`. The smaller the numbers I use for RGB (Red Green Blue) the less bright the colors will be!

![owl pupils color](/Assets/owl-pupils-color.png)

# Pupils
We left the numbers for the right eye's pupil positon and size as `0000`. Its your job to fill them in!

![owl pupils shapes](/Assets/owl-pupils-shapes.png)

# Pupil outline
The owl's eyes look fabulous.

![owl eyes unfinished](/Assets/owl-eyes-unfinished.png)

But they could be better! They really need some yellow around them. For this we can add an outline to the pupils.

![owl eyes finished](/Assets/owl-eyes-finished.png)

We see 2 new commands here.

```java
stroke(reg, gree, blue);
```

The `stroke` command sets the color of the outline or "stroke" (as in a painting brush's stroke).

```java
strokeWeight(width);
```

The `strokeWeight` command sets the width of the stroke.