float r;
float g;
float b;
float a;
float diam;
float x;
float y;
float m;
float n;

void setup(){
size(1000,1000);
background(255);
rectMode(CENTER);
ellipseMode(CENTER);
}

void draw(){
  r = random(255);
  g = random(255);
  b = random(255);
  a = random(255);
  x = random(width);
  y = random(height);
  m = random(width);
  n = random(height);
  diam = random(50);
  
  strokeWeight(diam);
  stroke(r,g,b,a);
  fill(r,g,b,a);
  ellipse(x,y,diam,diam);
  rect(m,n,diam,diam);
  line(x,y,m,n);

}
void mousePressed(){
  background(r,g,b,a);
}
