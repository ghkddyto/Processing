# Report 5-2
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
  if(i>width-100/2*8) b=-1;
  if(i<0) b=1;
  i = i+a*b;
  if(keyPressed) a = key-'0';
}
```

### 코드 설명
* text로 생성한 글자가 i의 좌표에 생성되고 i의 좌표를 왼쪽에서 오른쪽으로 왔다갔다하게 함으로써
생성된 글자 배너가 좌우로 움직이는 코드입니다.
