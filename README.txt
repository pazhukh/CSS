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

//другий спосіб
video {
	height: 100%;
	object-fit: cover;
	z-index: 0;
	width: 100%;
	background: no-repeat;
	background-size: cover;
	position: relative;
	background-position: center center;
	margin: auto;
	left: 0;
	right: 0;
	bottom: 0;
	top: 0;
}

*****************************************************************************************
похилі секції
	&::before{
		content: '';
		position: absolute;
		top: -5%;
		left: -5%;
		height: 100px;
		width: 110%;
		background-color: white;
		transform: rotate(-2deg);
	}
	&::after{
		content: '';
		position: absolute;
		bottom: -5%;
		left: -5%;
		height: 100px;
		width: 110%;
		background-color: white;
		transform: rotate(-2deg);
	}


******************************************************************************************

//responsive square
https://spin.atomicobject.com/2015/07/14/css-responsive-square/

//вибрати два останні елементи
&:nth-last-of-type(-n+2)

******************************************************************************************

//змінюємо стандартні стилі autocomplite -webkit браузери
input:-webkit-autofill,
input:-webkit-autofill:hover, 
input:-webkit-autofill:focus
input:-webkit-autofill, 
textarea:-webkit-autofill,
textarea:-webkit-autofill:hover
textarea:-webkit-autofill:focus,
select:-webkit-autofill,
select:-webkit-autofill:hover,
select:-webkit-autofill:focus {
	-webkit-text-fill-color: $lightBlack;
	-webkit-box-shadow: 0 0 0px 1000px white inset;
	transition: background-color 5000s ease-in-out 0s;
}

*******************************************************************************************

//input при кліку placeholder іде на верх
input:not([value=""]) ~ b, input:focus ~ b{
	top: -10px;
	color: $gold;
	font-size: 12px;
} 
//js
$("input").each(function(){
			$(this).on('keyup', function(){
				$(this).attr('value', $(this).val());
			})
		});

//нижній бордер зєвляється
input:focus ~ span{
		transform: scale(1);
	}
