# Report 2-2
## 안동대학교 컴퓨터공학과 황요새

```
PFont f;
void setup(){
  size(700,800);
 
  f = createFont("굴림", 64);
  textFont(f);
}

int i,a=1,b=1 ;
void draw(){
  background(0,128,255);
  fill(255,174,201);
  text("안동대 컴공 사랑합니다" ,10,i=i+a);
  if(i>800) i=0;
  if(keyPressed) a = key-'0';
}
```
### 리포트소감.
 * 방향 위치 속도를 마음대로 조절하니 프로세싱에 자신감이 생겼습니다!
