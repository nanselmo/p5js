# p5js

## Incrementing with Variables
```js
var xPos=40;
var yPos=50;
var gColor=0;
function setup() {
  createCanvas(600, 400);
}

function draw() {
    fill(0,gColor,0);
    ellipse(xPos,yPos,10,10);
    xPos=xPos+10;
    yPos=yPos+20;
    gColor=gColor+50;
  
}
```
## Mouse Paint w/ Random Color
```js
function setup() {
  createCanvas(600, 400);
}


function draw() {
  fill(0,random(200,255),225);
  ellipse(mouseX,mouseY,25,25);

}
```
##Speed with pmouseX
```js
var speed=0;
function setup() {
  createCanvas(600, 400);
}


function draw() {
  fill(0,random(100,255),225);
  ellipse(mouseX,mouseY,speed,speed);
  //define speed as the difference in the mouse's x position
  speed=mouseX-pmouseX

}
```
