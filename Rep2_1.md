```
void setup(){
  size(800,300);
  textSize(100);
}

int i,a=1,b=1 ;
void draw(){
  background(0,128,255);
  text("Graphics" ,i, 175);
  if(i>width) b=-1;
  if(i<0) b=1;
  i = i+a*b;
  if(keyPressed) a = key-'0';
}
```
