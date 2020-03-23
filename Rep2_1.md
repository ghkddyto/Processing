# Report 2-1
## 안동대학교 컴퓨터공학과 황요새
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
