# Stanford CS101 

This is a self-paced introductory course to Computer Science by Nick Parlante - Stanford University. It introduces a complete beginner to the subject by taking them through the basic ideas of how computers work - the nature of computers, what they can and can't do, code, hardware, security, analog vs digital, memory, and other computer concepts and jargon. 

Link to the course: [Computer Science 101](https://learning.edx.org/course/course-v1:StanfordOnline+CSX0001+1T2020/home).

**Note:** 
* Keep in mind that this course uses **JavaScript** for exercises.

# Code Writing: Why Code and how does it work in a Computer?

Humans need a language to communicate with machines. This is what computer programming languages are for - to tell the computer what to do. There are numerous languages - JavaScript, Python, C++, PHP, etc.
Using the code or programming language, you write algorithms that are basically commands for the machine to perform. Algorithm sets the rules and steps for the machine to perform a particular task.      
Example of code:
```javascript
print(1, 2);
```
If you run this code, the output will be 1 2. Which means the machine understands that the user is giving him command to print 1 2. 

## What is a string?
In computer science, a string is **a series of letters or a sequence of characters**. In JavaScript, a string is written within double quotes:
```javascript
print("This is a string."); 
```
It will print (display): `This is a string.`
Strings are used to hold urls or paragraphs. 
**Strings and numbers are the two most common data types in computer code.**

**Comments** are written to make notes for yourself (the programmer) within the code. The computer will ignore them when you run the code.
Again in JavaScript, comments are written using two forward slashes.
```javascripts
\\This is a comment and the computer will ignore when you run your code
```
## Syntax error 
Everyone runs into a syntax error. It basically means that the computer does not understand your command because you made a mistake in typing the syntaxes and the computer fails to do what you want it to do. For the most part, the error messages are straight forward and clear, but they can be subtle too. But nothing to be ashamed; it happens to everyone. 

## But what are Code Variables?
Okay, I understand what are strings, but whar are variables then?
In computer science, variables are used as a way of assigning values to a box (memory) so that you can retrive it later whenever you want use it. And that saves you from repeatedly writing the value.
For example, if you assigned `x = this is funny as hell`, you will be able to write `x` whenever you want to write `this is funny as hell` and the computer will pull the value which is `this is funny as hell`.  
Another example, say `x = 700`
This stores the value 700 into the variable (i.e. box) **x**, so that you can conveniently retrive them in th efuture.
**Variables are used to store information to be referenced and manipulated in a computer program.**

# How digital image works in Computer?
Digital images comprises of pixels. They are small boxes of colors.

1 mega pixex = 1 million pixels.

By using three natural colors (lights) - Red, Green, Blue (RGB) - you can make any color by combining (mixing) them together in fifferent ways.

So, each coolor (pixel) can be indicated by the numbers of the three colors- RGB. So you can say, every color is comprises of  three numbers.
Every pixel shows one color and that color can be captured by three no.

For example, you can say a pixel has 20, 50, 100. That means it has 20 red, 50 green, and 100 blue, which will give you a particular color. The no indicates the intensity of the color. Let's say 255 is the most intense, and if red is 250, then the most red is present in the pixel. The intensity starts with 0 = dark (no light or color, you can see anything).  If all three colors are at zero, you get black; if all three colors are at 255, you get white.

## Image Code

PNG is an image format, Portable Network Graphics

### Let's break down this image code: Remember, this is JavaScript
```javascript
image = new SimpleImage("x.png");
image.setZoom(20);
print(image);
```
*The image "x.png" is very simple -- it's a very small black square with a white "x" at its center.*

**What is this code (command) telling the computer to do?**
This is a three-line program
image = new SimpleImage("x.png"); -- this line calls the computer to load the x.png image into a variable
image.setZoom(20); -- this line calls the computer to set the zoom option to 20 (you can choose 10, 20, 30, etc). It calls the setZoom functions. There are others functions like this.
print(image); -- This line calls the computer to print image to the right.
If you run the code, you will see something like this:

<image src="https://github.com/rin2021/Computer-Science-101-/blob/main/Src/Assets/x.png" alt="x.png" width="60" height="60">

Zoom: each pixel is shown at 20x size here.
Our first image code example loads the `x.png` image and prints it.
  
**Another example:**
```javascript
image = new SimpleImage("x.png");
image.setZoom(20);
pixel = image.getPixel(1, 1);
pixel.setRed(250);
print(image);
```  
This will set the pixel number 1,1 of the image `x.png` to red whith the intensity of 250 (which is very red).
If you run the code, it will look something like this: 
  
<image src="https://github.com/rin2021/Computer-Science-101-/blob/main/Src/Assets/red.png" alt="red pixel" width="60" height="60">  
  
## Image For-Loop

  In computer science, a for-loop is a control flow statement for specifying iteration, which allows code to be executed repeatedly. 
  
  In this case, we are applying the concept of a for-loop to image processing.
  
With for-loop, you can avoid writing the code manually for each pixel as in:
`pixel = image.getPixel(1, 1);
pixel.setRed(250);`

This is not practical way to process a whole image.   

Using for-loop, you can just write a few line of code that capture the changes we want to make.
  
  
