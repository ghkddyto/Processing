# Report 5-5
## 안동대학교 컴퓨터공학과 황요새
```
PShape bot;

void setup() {
  size(640, 360);
  bot = loadShape("bot1.svg");
} 

void draw() {
  background(102);
  translate(width/2, height/2);
  float zoom = map(mouseX/4+mousey/4, 0, width, 0.1, 4.5);
  scale(zoom);
  shape(bot, -140, -140);
}

```

### 코드 설명
* svg파일로 미리 만들어둔 도형을 불러와 활용할수 있게 합니다.
* 만들어진 도형이 마우스의 위치에 따라 크기가 변하게 합니다.
