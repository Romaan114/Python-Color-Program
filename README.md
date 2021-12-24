# Python-Color-Program


# Program1 Synopsis
A spirograph is a very interesting geometrical figure which is often symmetrical to both the axes. It produces mathematical roulette curves of the variety technically known as hypotrochoids and epitrochoids. Here, we’ve used a range of colors to draw circles, you can use your combination as per your color choice.
We have programmed a spirography using python turtle in this program
The Code For the Following Program is:


#Import the turtle library for
#drawing the required curve

import turtle as tt

#Set the background color as black,
#pensize as 2 and speed of drawing

#curve as 10(relative)
tt.bgcolor('black')
tt.pensize(2)
tt.speed(10)

#Iterate six times in total
for i in range(6):

	# Choose your color combination
	for color in ('red', 'magenta', 'blue',
				'cyan', 'green', 'white',
				'yellow'):
		tt.color(color)
		
		# Draw a circle of chosen size, 100 here
		tt.circle(100)
		
		# Move 10 pixels left to draw another circle
		tt.left(10)
	
	# Hide the cursor(or turtle) which drew the circle
	tt.hideturtle()




# Program2 Synopsis
# First Part:
First, import everything from the turtle module. Then, set a turtle screen into a variable “s”. Set the screen size to (700, 1000) and the speed to 5.

Define a function myPosition() with the parameters “x, y”. Here, pick the pen up as we are not ready to draw. Go to the position as in (x, y). Put the pen down. Set the pen size to 2.

# Second Part:
Define a function named ankur() for the shorts of our drawing. Here, set the fill color as ‘#ffec40’. Begin the fill. Now, move the turtle right at 25 units, forward at 20, right at 45, and again forward at 20 units. Move the turtle left at a value of 70 units and again forward at 90 units. Likewise, move the turtle left at 95 units, forward at 90, left at 95, forward at 75, left 85, and again forward at 175 units. Similarly, move it left at 85 units, forward at 75, and as in the code. End the fill.


Define another function named leftLeg(). Here, set the position to (-39, -25). Set the fill color as ‘#ffd699’. Begin the fill. Move the turtle right at 89 degrees, forward at 25, right at 90, and forward at 50. Likewise, move the turtle right at 90 units, forward at 20, right at 85, and again forward at 50 units. End the fill.


Define other functions for different body parts and. You can see that the most used functions and methods are forward, left, right, begin_fill(), fillcolor(), and endfill().

# Third Part (Assemble the parts):
Going on with defining and implying all the function, now, create another one named allLegs(). Inside this function, call all the functions that are associated with drawing the parts of the legs of the cartoon. The functions are : leftLeg(), leftSock(), leftShoe(), rightLeg(), rightSock(), rightShoe().


Likewise, create a function named allHands that assembles the parts of the hands of the cartoon. The functions are: rightHand(), leftHand(), myBis() and leftHand2().


Similarly, create another function named allEyebrows(). Here, call the myEyebrow() function with the arguments (-8, 300), right at 90 units, again myEyebrow with the arguments (72, 300), myEyelid() with the arguments (-8, 270), left with 15 units, and at last myEyelid() with (68, 265).


Now, create a function allEyes() and assemble myallEyes1(17, 275) and myallEyes2(95, 270).


# Last Part:
Here, call all the functions that were assembled in the above part. Here call the function: ankur(), allLegs()myShirt(), myHead() ,allHands(), myMouth(), allEyebrows(), allEyes(), myRobot().


After it is done, hide the turtle with the method ht() and finish the code with the done() method.



# Code:

from turtle import *
#import time
s=Screen()
s.screensize(700,1000)
speed(5)
def myPosition(x, y):
    penup()
    goto(x, y)
    pendown()
#time.sleep(10)
#ht()
pensize(2)
def ankur():
    fillcolor('#ffec40')
    begin_fill()
    right(25)
    forward(20)
    right(45)
    forward(20)
    left(70)
    forward(90)
    left(95)
    forward(75)
    left(85)
    forward(175)
    left(85)
    forward(75)
    left(95)
    forward(90)
    left(85)
    forward(18)
    end_fill()

def leftLeg():
    myPosition(-39,-25)
    fillcolor("#ffd699")
    begin_fill()
    right(89)
    forward(25)
    right(90)
    forward(50)
    right(90)
    forward(20)
    right(85)
    forward(50)
    end_fill()

def leftSock():
    myPosition(-36,-78)
    fillcolor("#ffffff")
    begin_fill()
    right(90)
    circle(80,13)
    right(110)
    forward(22)
    right(85)
    forward(19)
    right(90)
    forward(21)
    end_fill()

def leftShoe():
    myPosition(-69,-112)
    fillcolor("#b5ae60")
    begin_fill()
    right(90)
    left(5)
    forward(56)
    left(105)
    forward(13)
    left(75)
    forward(20)
    right(90)
    forward(15)
    circle(10,15)
    left(80)
    forward(4)
    circle(10,15)
    left(40)
    circle(20,15)
    forward(10)
    right(45)
    forward(15)
    circle(25,25)
    end_fill()

def rightLeg():
    myPosition(60,-28)
    fillcolor("#ffd699")
    begin_fill()
    #right(90)
    left(128)
    forward(25)
    right(95)
    forward(55)
    right(90)
    forward(20)
    right(85)
    forward(55)
    end_fill()

def rightSock():
    myPosition(64,-79)
    fillcolor("#ffffff")
    begin_fill()
    right(90)
    circle(90,14)
    right(110)
    forward(23)
    right(90)
    forward(15)
    right(80)
    forward(21)
    end_fill()

def rightShoe():
    myPosition(64,-108)
    fillcolor("#b5ae60")
    begin_fill()
    right(100)
    forward(56)
    left(160)
    forward(25)
    right(68)
    forward(17)
    left(90)
    circle(18,15)
    forward(5)
    left(75)
    forward(11)
    right(85)
    forward(20)
    left(45)
    circle(10,30)
    left(25)
    forward(5)
    end_fill()

def myShirt():
    myPosition(-75,48)
    fillcolor("red")
    begin_fill()
    left(72)
    forward(185)
    left(87)
    forward(75)
    right(68)
    circle(20,8)
    circle(300,23)
    left(90)
    circle(35,17)
    right(38)
    circle(35,17)
    left(58)
    forward(75)
    right(12)
    forward(140)
    right(40)
    forward(93)
    left(120)
    circle(-20,65)
    left(75)
    forward(10)
    left(23)
    forward(88)
    #circle(-80,10)
    right(31)
    forward(87)
    right(180)
    forward(108)
    right(180)
    forward(104)
    circle(10,70)
    end_fill()

def myHead():
    myPosition(-20,295)
    left(20)
    pensize(2)
    fillcolor('#fcc6a0')
    begin_fill()
    right(90)
    forward(40)
    right(90)
    circle(50,80)
    left(10)
    circle(50,80)
    left(2)
    circle(200,50)

    left(48)
    forward(60)
    #left(20)
    circle(45,60)
    right(5)
    circle(100,85)
    end_fill()
    fillcolor('black')
    begin_fill()

    pensize(2)
    right(170)
    circle(-100,165)
    right(78)
    forward(26)
    right(87)
    forward(55)
    circle(45,60)
    right(5)
    circle(100,85)
    end_fill()

    fillcolor('#fcc6a0')
    begin_fill()
    right(180)
    circle(-100,105)
    right(37)
    forward(49)
    pensize(2)
    left(130)
    forward(30)
    #right(5)
    circle(-10,70)
    right(50)
    #circle(10,10)
    forward(36)
    right(80)
    forward(50)
    pencolor('#fcc6a0')
    right(90)
    forward(30)
    
    end_fill()

def rightHand():
    #left(35)
    myPosition(197,209)
    pencolor('black')
    fillcolor('#fcc6a0')
    begin_fill()
    right(45)
    forward(6)
    left(55)
    forward(20)
    circle(-5,70)
    right(100)
    forward(18)
    left(105)
    forward(18)
    circle(-5,70)
    right(100)
    forward(18)
    left(145)
    forward(15)
    circle(-5,70)
    right(100)
    forward(18)

    left(150)
    forward(13)
    circle(-5,70)
    right(100)
    forward(15)

    left(150)
    forward(10)
    circle(-5,70)
    right(100)
    forward(12)
    circle(60,10)
    left(45)
    forward(6)
    right(90)
    forward(10)
    end_fill()

def leftHand():
    myPosition(-94,242)
    fillcolor('#fcc6a0')
    begin_fill()
    right(10)
    forward(6)
    left(90)
    penup()
    forward(12)
    pendown()
    left(90)
    forward(8)
    left(90)
    forward(12)
    end_fill()

def myBis():
    myPosition(-103,291)
    right(90)
    fillcolor('#02d302')
    begin_fill()
    right(90)
    forward(55)
    left(80)
    forward(12)
    left(10)
    forward(17)
    left(10)
    forward(12)
    left(80)
    forward(55)
    left(80)
    forward(12)
    left(10)
    forward(17)
    left(10)
    forward(12)
    left(80)
    left(80)
    forward(12)
    left(10)
    forward(17)
    left(10)
    forward(12)
    end_fill()
    penup()
    right(100)
    forward(20)
    right(90)
    forward(14)
    pendown()
    pencolor('#9c5e4a')
    fillcolor('#9c5e4a')
    begin_fill()
    for i in range(5):
        forward(15)
        right(144)
    end_fill()
    penup()
    forward(27)
    left(90)
    forward(16)
    left(90)
    forward(7)
    pendown()
    fillcolor('#9c5e4a')
    begin_fill()
    for i in range(5):
        forward(10)
        right(144)
    end_fill()
    penup()
    forward(20)
    right(90)
    forward(5)
    pendown()
    fillcolor('#9c5e4a')
    begin_fill()
    for i in range(5):
        forward(10)
        right(144)
    end_fill()
    penup()
    right(180)
    forward(6)
    pendown()
    fillcolor('#9c5e4a')
    begin_fill()
    for i in range(5):
        forward(10)
        right(144)
    end_fill()

def leftHand2():
    myPosition(-112,284)
    pencolor('black')
    fillcolor('#fcc6a0')
    begin_fill()
    right(180)
    forward(31)
    left(90)
    for i in range(2): 
        circle(4,90) 
        #circle(4//2,45)
    for i in range(3):
        right(180)
        for i in range(2): 
            circle(4,90)
    end_fill()

def myMouth():
    myPosition(-25,200)
    left(65)
    fillcolor('#77332e')
    begin_fill()
    #circle(20)
    #forward(20)
    for i in range(2): 
        circle(25,90) 
        circle(25//2,90)
    end_fill()

def myEyebrow(x,y):
    myPosition(x,y)
    pensize(18)
    right(150)
    forward(25)
    right(90)
    for i in range(1):
        right(45)
        dot(15)
    left(55)
    forward(25)
    for i in range(1):
        right(45)
        dot(15)

def myEyelid(x,y):
    myPosition(x,y)
    pensize(2)
    left(170)
    circle(-23,180)

def myallEyes1(x,y):
    myPosition(x,y)
    right(90)
    fillcolor('#000000')
    begin_fill()
    circle(18)
    end_fill()
    left(90)
    penup()
    forward(19)
    right(90)
    forward(7)
    pendown()
    fillcolor('#ffffff')
    begin_fill()
    left(90)
    circle(9)
    end_fill()

def myallEyes2(x,y):
    myPosition(x,y)
    right(90)
    fillcolor('#000000')
    begin_fill()
    circle(18)
    end_fill()
    left(90)
    penup()
    forward(19)
    right(90)
    forward(8)
    pendown()
    fillcolor('#ffffff')
    begin_fill()
    left(90)
    circle(9)
    end_fill()

def myRobot():
    myPosition(155,-105)
    left(93)
    color('red')
    pensize(7)

    begin_fill()
    forward(50)
    left(90)
    forward(50)
    left(90)
    forward(50)
    left(90)
    forward(50)
    left(90)
    end_fill()


    color('white')
    penup()
    left(90)
    forward(30)
    right(90)
    forward(12)
    pendown()
    pensize(3)
    circle(5)
    penup()
    forward(25)
    pendown()
    circle(5)

    penup()
    right(90)
    forward(20)
    right(90)
    pendown()

    begin_fill()
    forward(23)
    right(90)
    forward(7)
    right(90)
    forward(23)
    right(90)
    forward(7)
    right(90)
    end_fill()

    penup()
    forward(25)
    right(90)
    forward(35)
    pendown()

    color('red')
    forward(30)
    penup()
    right(90)
    pendown()
    begin_fill()
    circle(5)
    end_fill()

def allLegs():
    leftLeg()
    leftSock()
    leftShoe()
    rightLeg()
    rightSock()
    rightShoe()
def allHands():
    rightHand()
    leftHand()
    myBis()
    leftHand2()
def allEyebrows():
    myEyebrow(-8,300)
    right(90)
    myEyebrow(72,300)
    myEyelid(-9,270)
    left(15)
    myEyelid(68,265)    
def allEyes():
    myallEyes1(17,275)
    myallEyes2(95,270)
ankur()
allLegs()
myShirt()
myHead()
allHands()
myMouth()
allEyebrows()
allEyes()
myRobot()
ht()
done()


Using turtle Library 


Learn Turtle 
