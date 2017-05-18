https://transfonter.org/  - трансформаці шрифтів

//посиціонуємо по центрі блока
position: absolute;
top: 50%;
left: 50%;
transform: translate(-50%, -50%);

//hover css
https://ianlunn.github.io/Hover/
https://github.com/IanLunn/Hover/blob/master/css/hover.css

//відео background на весь екран(стилі для тегу <video>)
.video {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
}
@media (min-aspect-ratio: 16/9) {
  .video {
    height: 300%;
    top: -100%;
  }
}
@media (max-aspect-ratio: 16/9) {
  .video {
    width: 300%;
    left: -100%;
  }
}
