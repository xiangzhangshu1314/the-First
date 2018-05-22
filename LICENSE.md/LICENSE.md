<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title>ball-3d</title>
		<style type="text/css">
			/**{padding: 0;margin: 0;}*/
body{background-color: cornflowerblue;}
#ball-box{
	height: 300px;
	width: 300px;
	
	position: absolute;
	top: 50%;
	left: 50%;
	margin: -150px 0 0 -150px;
}
#ball{height: 100%;
transform-style: preserve-3d;
animation: rotate3d 20s infinite linear;
}
@-webkit-keyframes rotate3d{
	0%{transform: rotateY(0deg);}
	100%{transform: rotateY(360deg);}
}

#ball>div{background-color: #f40;
	border: 2px solid white;
	height: 100%;
	width: 100%;
	position: absolute;
	border-radius: 100%;
	}
.line-1{
	transform: rotateY(0deg);
}	
.line-2{
	transform: rotateY(36deg);
}	
.line-3{
	transform: rotateY(72deg);
}	
.line-4{
	transform: rotateY(108deg);
}	
.line-5{
	transform: rotateY(144deg);
}	
#ball::after{
	content: '';
	width: 1px;
	height: 500px;
	background-color: #ff0;
	display: block;
	transform: translateX(150px) translateY(-100px);
}
/*编辑器不支持，谷歌浏览器里能看到旋转的效果*/

		</style>
	</head>
	<body>
		<div id="ball-box">
		<div id="ball">
			<div class="line-1"></div>
			<div class="line-2"></div>
			<div class="line-3"></div>
			<div class="line-4"></div>
			<div class="line-5"></div>
		</div>
		</div>
	</body>
</html>
