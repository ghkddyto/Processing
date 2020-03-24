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
  if(i>width-100/2*8) b=-1;
  if(i<0) b=1;
  i = i+a*b;
  if(keyPressed) a = key-'0';
}
```

### 리포트 소감
* 지금까지 배운 코딩은 명령창만 출력되서 조금 심심한 느낌이 있었는데 직접 만든 그래픽이 움직이는걸 보니 너무 재밌습니다!
* 심재창 교수님 사랑합니다♡♡♡
