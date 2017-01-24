# p5js

##References

Code modified from
* [Daniel Shiffman p5 tutorial](http://wykhuh.github.io/shiffman-p5-tutorials/)
* [Learning Processing Book from Daniel Shiffman](http://learningprocessing.com/examples)


## Incrementing with Variables
```js
var xPos=0;
var yPos=0;
var gColor=0;
function setup() {
  createCanvas(600, 400);
}

function draw() {
  //uncomment out the background will redraw the background each time so the previous elipse doesn't show
  //background(0,0,0);
  fill(0,gColor,0);
  ellipse(xPos,yPos,10,10);
  xPos=xPos+5;
  yPos=yPos+10;
  gColor=gColor+10;

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
## Speed with pmouseX
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

## Change Color on Conditional Statement testing X value

```js
function setup() {
  createCanvas(600, 400);
}

function draw() {
  if (mouseX>150){
    redColor=100;
  } else if (mouseX < 150) {
    redColor=0;
  }
  fill(redColor,random(0,225),225);
  ellipse(mouseX,mouseY,10,10);
  
}
```
