# Report 5-1
## 안동대학교 컴퓨터공학과 황요새
```
void setup(){
  size(500,500);
  background(255);
  stroke(0);
  strokeWeight(16);
}
void draw(){
  if(mousePressed)
      line(pmouseX,pmouseY,mouseX,mouseY);  
}

```

### 코드 설명
흰 바탕의 스케치 위에 마우스로 클릭한곳에 검은 선을 그릴수 있는, 즉 펜을 만드는 코드입니다.
