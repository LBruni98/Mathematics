# Mathematics
This repo is dedicated towards mathematical methodologies and the sort. For mathmatical code algorithms, the repo can be found [here.](https://github.com/LBruni98/Maths-Code-Samples)

### Probability Theory

#### The probability of a random integer being divisible by 5
To Calculate the probability of a random interger being divisible by 5, you'll first have to take note of each of the numbers that end in 5 and of course these numbers can be divided by 5; 5, 10, 15, 20, 25, basically the 5 times table. Numbers in between are not probable to be dividable by 5 and hence, this gives the probability 1/5.

![Probability](https://github.com/LBruni98/Mathematics/blob/master/Probability.PNG)

####  How to calculate the greatest common divisor and least a common multiple of a given pair of numbers
GCD means the **G**reatest **C**ommon **D**ivisor which is the largest number that divides any given numbers. To calculate this, let's say I needed to find the GCD of both 45 and 54. I would first need to find the divisors of these numbers. The divisors are as followed...
* 45: 1, 3, 5, *9*, 15, 45
* 54: 1, 2, 3, 6, *9*, 18, 27, 54

Next would be to find the greatest number, which is the highest number that is shared in the two lists. Here, the number is *9*.

LCM means the **L**east **C**ommon **M**ultiple and this is the smallest number that is basically a mulitple of any given number. So, if I were to find the LCM of both 6 and 8, the first thing I would do would be to run by the multiples of both numbers. Here they are as followed...
* 6: 6, 12, 18, *24*, 30, ...
* 8: 8, 16, *24*, 32, 40, ...

Next would be to find the smallest matching number from both lists, which would be *24*.

### Conditional Probability
Condition probability, is the probability that event A has occurred in a random experiment, taking into account that event b has definitely occured. The following formula for the rule of Conditional Probability:

![Conditional](https://github.com/LBruni98/Mathematics/blob/master/Conditional%20Probability.PNG)

#### What would the probability of a 7 be when rolling two dice?
The probability of having a seven when rolling two dice would be 6/36. The outcome was found adding two of each value of the two dice and then counting the amount of times a seven would appear. Hence, the sum for the possible outcome is six, meaning that the probability of rolling a seven when rolling two dice is 6/36 or 1/6.

### Vectors to Define Shapes
A vector describes the movement from one point to another and has two independant properties: the magnitude and direction.

![Vectors](https://github.com/LBruni98/Mathematics/blob/master/Vectors.PNG)

Vectors can be used to create shapes by identifying parameters. This formula demonstrates the creation of shapes by using vector methods.

```html
<html>
<body>

<canvas id="myCanvas" width="300" height="150" style="border:1px solid #d3d3d3;"></canvas>

<br>
<button onclick="move(1)">LEFT</button>
<button onclick="move(2)">UP</button>
<button onclick="move(3)">DOWN</button>
<button onclick="move(4)">RIGHT</button>
<br>
<button onclick="move(5)">DIAGONAL RIGHT DOWN</button>
<button onclick="move(6)">DIAGONAL RIGHT UP</button>
<br>
<button onclick="move(7)">DIAGONAL LEFT DOWN</button>
<button onclick="move(8)">DIAGONAL LEFT UP</button>
<br>
<button onclick="shape()">SHAPE?</button>


<script>
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
ctx.beginPath();

var curX=parseInt(prompt("Please enter the initial X"));;
var curY=parseInt(prompt("Please enter the initial Y"));;

function move(dir){
var mag = parseInt(prompt("Please enter the magnitude"));

if(dir==1){
  //left
  ctx.moveTo(curX, curY);
  curX = curX-mag;
  ctx.lineTo(curX, curY);  
  alert("Vector Direction: Left / Vector Magnitude: "+mag);
}else if(dir==2){
  //up
  ctx.moveTo(curX, curY);
  curY = curY-mag;
  ctx.lineTo(curX, curY);  
  alert("Vector Direction: Up / Vector Magnitude: "+mag);
}else if(dir==3){
  //down
  ctx.moveTo(curX, curY);
  curY = curY+mag;
  ctx.lineTo(curX, curY);  
  alert("Vector Direction: Down / Vector Magnitude: "+mag);
}else if(dir==4){
  //right
  ctx.moveTo(curX, curY);
  curX = curX+mag;
  ctx.lineTo(curX, curY);  
  alert("Vector Direction: Right / Vector Magnitude: "+mag);
}else if(dir==5){
  //diagonal right down
  ctx.moveTo(curX, curY);
  curX = curX+mag/2;
  curY = curY+mag/2;
  ctx.lineTo(curX, curY);  
  alert("Vector Direction: Diagonal Right Down / Vector Magnitude: "+mag);
}else if(dir==6){
  //diagonal right up
  ctx.moveTo(curX, curY);
  curX = curX+mag/2;
  curY = curY-mag/2;
  ctx.lineTo(curX, curY);  
  alert("Vector Direction: Diagonal Right Up / Vector Magnitude: "+mag);
}else if(dir==7){
  //diagonal left down
  ctx.moveTo(curX, curY);
  curX = curX-mag/2;
  curY = curY+mag/2;
  ctx.lineTo(curX, curY);  
  alert("Vector Direction: Diagonal Left Down / Vector Magnitude: "+mag);
}else if(dir==8){
  //diagonal left up
  ctx.moveTo(curX, curY);
  curX = curX-mag/2;
  curY = curY-mag/2;
  ctx.lineTo(curX, curY);  
  alert("Vector Direction: Diagonal Left Up / Vector Magnitude: "+mag);
}

ctx.stroke();

}

function shape(){
  var shape = prompt("Is this a shape Y/N?");

  if(shape=='Y'){
      prompt("What shape?");
  }else {
      alert("Keep drawing!");
  }
}

</script>

</body>
</html>
```

### Rate of Change
Rate of change describes the average rate at which a quantity changes with respect to something else. For instance, miles per hour is calculated by dividing the number of miles to the amount of time it takes to travel said miles.

The average rate of change function calculates the amount of change in one quantity divided by the corresponding change in the other. We can define this rate of change of a function from a to x, shown here as:

![Rate of Change](https://github.com/LBruni98/Mathematics/blob/master/formulaRC.png)

#### First Example
![Rate of Change 1](https://github.com/LBruni98/Mathematics/blob/master/Rate%20of%20Change%201.PNG)

Answer in Binary: 1

#### Second Example
![Rate of Change 2](https://github.com/LBruni98/Mathematics/blob/master/Rate%20of%20Change%202.PNG)

Answer in Hexadecimal: 0334

Conversion Table:

|Decimal|Hex|Binary|
|-------|---|------|
|0|0|0000|
|1|1|0001|
|2|2|0010|
|3|3|0001|
|4|4|0100|
|5|5|0101|
|6|6|0110|
|7|7|0111|
|8|8|1000|
|9|9|1001|
|10|A|1010|
|11|B|1011|
|12|C|1100|
|13|D|1101|
|14|E|1110|
|15|F|1111|

### Integral Calculus to Solve Practical Problems Involving Area
This is a branch of mathematics that is deals with properties and application of intergrals, which in turn is the space under a graph or area of curvature and applying this can aid in describing or finding displacement or area of said space.

![Area](https://github.com/LBruni98/Mathematics/blob/master/Integral%20Calculus%20Area.PNG)

Completing an average equation requires more than one area to be calculated. To do this, we need to take the above graph and place rectangles in the area to figure out each one, and helping us find out the area.

![Area with Rectangles](https://github.com/LBruni98/Mathematics/blob/master/Integral%20Calculus%20Area%20Rectangles.PNG)

Below is the forumla for calculating integral calculus:

![Formula](https://github.com/LBruni98/Mathematics/blob/master/ICFormula.PNG)

The symbol ∫, represents integration within the formula and is where the integral is found.

The 'a' and 'b' letters placed on the other side of the ∫ symbol represent that the caculations are going from 'a' to 'b'. The symbol 'dx' shows the differential of the 'x' and this also showing us the variable of integration also being 'x'. The area is found from the 'x' axis curve, making 'x' the intgral.
