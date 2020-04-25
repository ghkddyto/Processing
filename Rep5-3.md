# Report 5-
## 안동대학교 컴퓨터공학과 황요새
```
void setup() {
  size(640, 360);
}

void draw() {
  background(102);
  
  pushMatrix();
  translate(width*0.2, height*0.5);
  rotate(frameCount / 200.0);
  fill(255,255,0);
  star(0, 0, 5, 70, 3); 
  popMatrix();
  
  pushMatrix();
  translate(width*0.5, height*0.5);
  rotate(frameCount / 400.0);
  fill(255,0,0);
  star(0, 0, 80, 100, 40); 
  popMatrix();
  
  pushMatrix();
  translate(width*0.8, height*0.5);
  rotate(frameCount / -100.0);
  fill(0,0,255);
  star(0, 0, 30, 70, 5); 
  popMatrix();
}

void star(float x, float y, float radius1, float radius2, int npoints) {
  float angle = TWO_PI / npoints;
  float halfAngle = angle/2.0;
  beginShape();
  for (float a = 0; a < TWO_PI; a += angle) {
    float sx = x + cos(a) * radius2;
    float sy = y + sin(a) * radius2;
    vertex(sx, sy);
    sx = x + cos(a+halfAngle) * radius1;
    sy = y + sin(a+halfAngle) * radius1;
    vertex(sx, sy);
  }
  endShape(CLOSE);
}
```

### 코드 설명

별을 만드는 star 함수를 미리 만들어 놓고 push&popMatrix로 여러가지의 별이 나오게 합니다.
star 함수안의 angle값을 바꿔 회전하는 속도를 조절할 수 있습니다.
