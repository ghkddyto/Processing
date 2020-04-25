# Report 5-4
## 안동대학교 컴퓨터공학과 황요새
```
void setup() {
  size(300, 300);
  background(255);

  fill(132,125,200);
  polygon(3, 50, 75, 50);
  fill(200,200,0);
  polygon(4, 170, 75, 50);

  fill(255, 204, 255);
  stroke(128, 0, 128);
  polygon(5, 50, 180, 50);

  fill(30,245,11);
  stroke(0);
  polygon(6, 170, 180, 50);
}

void polygon(int n, float cx, float cy, float r) {
  float angle = 360.0 / n;

  beginShape();
  for (int i = 0; i < n; i++) {
    vertex(cx + r * cos(radians(angle * i)),
      cy + r * sin(radians(angle * i)));
  }
  endShape(CLOSE);
}
```

### 코드 설명
* 다각형을 만들어주는 polygon 함수를 미리 생성합니다.
* 각의 수와 각의 크기 , 도형의 크기 등을 설정해 원하는 도형들을 생성합니다.
