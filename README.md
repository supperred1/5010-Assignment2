# 5010-Assignment2

```javascript
function setup() {
  createCanvas(400, 400);
}

function draw() {
  background(mouseX,mouseY,mouseX-mouseY);
  fill(mouseY,mouseX,mouseY-mouseX);
  noStroke();
  ellipse(200,200,300,300)
  fill(mouseY-mouseX,mouseX-mouseY,mouseX);
  ellipse(mouseX,mouseY,100,100);let offsetXX = random(-5, 5);
    let offsetYY = random(-5, 5);
    stroke(random(255), random(255), random(255));
    ellipse(mouseX + offsetXX, mouseY + offsetYY, 250, 250);
  noStroke();
  ellipse(mouseX,mouseY,200,200)
  fill(255,0,0);
  noStroke();
  ellipse(mouseX,mouseY,100,100);let offsetX = random(-5, 5);
    let offsetY = random(-5, 5);
    stroke(random(255), random(255), random(255));
    ellipse(mouseX + offsetX, mouseY + offsetY, 80, 80);
  stroke(255,150,150);

  
  mousePressed();
  
  }
function mousePressed(){
    if(mouseIsPressed){
      stroke(30,255,255)
      line(mouseX,mouseY,pmouseX,pmouseY);
      let size = 20
      strokeWeight(size);
      for (let i = 0; i < 5; i++) {
      let x = mouseX + random(-200, 200);
      let y = mouseY + random(-200, 200);
      stroke(random(255), random(255), random(255));
      point(x, y);
  }      
      
    }
  }
```
### I need a spherical object resembling an eye that can follow the movement of the mouse. When the mouse is clicked, a glitch-like flickering pattern should appear around the sphere, accompanied by the generation of numerous small spheres.
####I wanted the drawn lines to fade over time, but the canvas keeps refreshing, and I'm not sure how to do it.
