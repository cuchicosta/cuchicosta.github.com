<!DOCTYPE html>
<html>
<head>
    <meta http-equiv="content-type" content="text/html; charset=UTF-8">
    <title>Cuchi Costa</title>

<style>


/* Fonts */

body {
    background-color:#000;
	background-image: url('Earth.jpg');
}

@font-face {
    font-family: 'BreeSerifRegular';
    src: url('fonts/BreeSerif-Regular-webfont.eot');
    src: url('fonts/BreeSerif-Regular-webfont.eot?#iefix') format('embedded-opentype'),
         url('fonts/BreeSerif-Regular-webfont.woff') format('woff'),
         url('fonts/BreeSerif-Regular-webfont.ttf') format('truetype'),
         url('fonts/BreeSerif-Regular-webfont.svg#BreeSerifRegular') format('svg');
    font-weight: normal;
    font-style: normal;
}

@font-face {
    font-family: 'BlanchCondensedInline';
    src: url('fonts/blanch/blanch_condensed_inline-webfont.eot');
    src: url('fonts/blanch/blanch_condensed_inline-webfont.eot?#iefix') format('embedded-opentype'),
         url('fonts/blanch/blanch_condensed_inline-webfont.woff') format('woff'),
         url('fonts/blanch/blanch_condensed_inline-webfont.ttf') format('truetype'),
         url('fonts/blanch/blanch_condensed_inline-webfont.svg#BlanchCondensedInline') format('svg');
    font-weight: normal;
    font-style: normal;

}

/* Menu Top */

.head {
	width: 100%;
	position: fixed;
}

.menu {
	background-image:url('header.png');
	position: relative;
	margin:0 auto;
	overflow: auto;
	width: 980px;
	height: 170px;
	top: 10px;
}

.menu ul {
	list-style-type: none;
	margin-top:38px;
	margin-left:90px;
}

.menu li {
	display: inline;
}

.menu li a {
	font-family: 'BlanchCondensedInline';
	font-size: 26px;
	text-decoration: none;
	color: #000;
	padding-top:22px;
	padding-bottom:2px;
	padding-left:15px;
	padding-right:15px;
	cursor:hand;
}

.menu li:nth-child(1) a { font-family: 'BlanchCondensedInline'; font-size:25px;padding-right:2px; padding-left: 2px; margin-bottom: -3px; position:relative; }
.menu li:nth-child(2) a { padding-right:2px; padding-left: 2px; margin-left: 60px; }
.menu li:nth-child(3) a { padding-right:2px; padding-left: 2px; margin-left: 57px; }
.menu li:nth-child(4) a { padding-right:2px; padding-left: 2px; margin-left: 69px; }
.menu li:nth-child(5) a { padding-right:2px; padding-left: 2px; margin-left: 65px; }

.menu li a:hover {
	border-bottom:2px dotted black;
}

.menu .headline {
	font-family:'BreeSerifRegular', Arial, sans-serif;
	font-size: 13px;
	word-spacing: 1px;
	color: #EDEDE3;
	margin-top: 28px;
	margin-left: 137px;
}  

.menu .headline a {
	text-decoration: none;
	padding: 2px 3px;
	color: #0099FF;
	-webkit-transition: background-color  0.1s linear;
	-moz-transition: background-color  0.1s linear;
	-o-transition: background-color  0.1s linear;
	transition: background-color  0.1s linear;
}

.menu .headline a:hover {
	background-color: #0099FF;
	color: #FFF;
	border-bottom: 3px solid black;
	cursor:hand;
}

.like a {
	font-family: 'BlanchCondensedInline';
	font-size: 26px;
	text-decoration: none;
	color: black;
	position:absolute;
	top:88px;
    right:51px;
}

.like a:hover {
	border-bottom:2px dotted black;
}


/* Keyboard */

.arrow-container {
	position: fixed;
	overflow: auto;
	width: 96px;
	height: 84px;
	bottom: 30px;
	right:15%;
}

a.arrow-top {
	background:url('arrows/key-top.png') no-repeat;
	background-position: 0 0;
	position: absolute;
	display: block;
	width:30px;
	height: 41px;
	overflow:hidden;
	text-indent: -3000px;
	top: 0px;
	left: 32px;
}

a:hover.arrow-top {
	background-position:0 -41px;
}

a.arrow-left {
	background:url('arrows/key-left.png') no-repeat;
	background-position: 0 0;
	position: absolute;
	display: block;
	width:30px;
	height: 41px;
	overflow:hidden;
	text-indent: -3000px;
	top: 43px;
	left: 0px;
}

a:hover.arrow-left {
	background-position:0 -41px;
}

a.arrow-bottom {
	background:url('arrows/key-bottom.png') no-repeat;
	background-position: 0 0;
	position: absolute;
	display: block;
	width:30px;
	height: 41px;
	overflow:hidden;
	text-indent: -3000px;
	top: 43px;
	left: 33px;
}

a:hover.arrow-bottom {
	background-position:0 -41px;
}

a.arrow-right {
	background:url('arrows/key-right.png') no-repeat;
	background-position: 0 0;
	position: absolute;
	display: block;
	width:30px;
	height: 41px;
	overflow:hidden;
	text-indent: -3000px;
	top: 43px;
	left: 66px;
}

a:hover.arrow-right {
	background-position:0 -41px;
}


/* Tool Tips */

.tooltip-procrastinate {
	background-color: #EDEDE3;
	border-bottom: 20px solid #999999;
	width: 130px;
	position: fixed;
	-moz-box-shadow: 0px 0px 5px #666;
	-webkit-box-shadow: 0px 0px 5px #666;
	box-shadow: 0px 0px 5px #666;
	padding:2px 10px 10px 10px;
	display: none;
	top:150px;
	left:63%;
} 

.tooltip-subscribe {
	background-color: #EDEDE3;
	border-bottom: 20px solid #999999;
	width: 130px;
	position: relative;
	-moz-box-shadow: 0px 0px 5px #666;
	-webkit-box-shadow: 0px 0px 5px #666;
	box-shadow: 0px 0px 5px #666;
	padding:2px 10px 10px 10px;
	float: left;
	display: none;
}


.tip {
	position: absolute;
	width: 21px;
	height: 8px;
	margin-top: -9px;
	margin-left: 50px;;
}



.title { 
    font-family: 'BreeSerifRegular';
	font-size:13px;
	float: left;
}

.border {
	padding: 0px;
	float:left;
	margin-top: -10px;
}

.categories {
    font-family: 'BreeSerifRegular';
	font-size:13px;
	text-align: left;
	display:block;
	width: 125px;
	float: left;
	margin-top:-10px;
}

.categories ul {
	list-style-type: none;
	padding: 0px;
}


.categories a {
	color: #0097FB;
	text-decoration: none;
	display:block;
	border-bottom: 1px dotted #666;
	padding-bottom: 3px;
	padding-left: 3px;
}

.categories a:hover {
	color: #FFF;
	background-color:#0097FB;
	border-bottom:0px solid #FFF;
	-webkit-transition: background-color  0.1s linear;
	-moz-transition: background-color  0.1s linear;
	-o-transition: background-color  0.1s linear;
	transition: background-color  0.1s linear;
}

.post-counter {
	text-align: right;
	color: #999;
	margin-right: 0px;
	float:right;
}

.post-counter:hover {
	color: #FFF;
}





.tooltip-bottom {
	background-color: #0099FF;
	border-bottom: 20px solid #1E90AF;
	width: 130px;
	position: fixed;
	-moz-box-shadow: 0px 0px 5px #666;
	-webkit-box-shadow: 0px 0px 5px #666;
	box-shadow: 0px 0px 5px #666;
	padding:10px 10px 0px 10px;
	float: left;
	display:none;
	bottom: 125px;
	right: 160px;
} 



.tip-bottom1 {
	position: absolute;
	width: 21px;
	height: 8px;
	bottom: -8px;
	margin-left: 53px;
}

.tip-bottom2 {
	position: absolute;
	width: 21px;
	height: 8px;
	bottom: -28px;
	margin-left: 53px;
}

.navigate {
    font-family: 'BreeSerifRegular';
	font-size:12px;
	color: #fff;
	text-align: center;
	display:block;
	width: 125px;
	float: left;
	margin-top: -2px;
}




</style>

	<script src="https://ajax.googleapis.com/ajax/libs/jquery/1.7.1/jquery.min.js"></script>
	
	<script>
		$(document).ready(function(){
			$('#arrow-top').hover(function(){
				$('#tooltip-bottom').toggle();
			}, function(){
				$('#tooltip-bottom').toggle();
			})
		});
		
		$(document).ready(function(){
			$('#procrastinate').click(function(){
				$('#tooltip-procrastinate').toggle();
			}, function(){
				$('#tooltip-procrastinate').toggle();
			})
		});
		
	</script>
</head>

<body>

<!-- Menu Top -->

<div class="head">
	<div class="menu">
		<ul>
			<li><a href="#">THE PORTABLE TOOLBOX OF A JOURNEYMAN</a></li>
			<li><a href="#">KNOW ME</a></li>
			<li><a href="#">WORK</a></li>
			<li><a href="#">HIRE</a></li>
			<li><a href="#">SEND ME A POSTCARD</a></li>
		</ul>	
		<p class="headline">I <a href="#">DESIGN</a> INTERACTIONS, <a href="#">COMMUNICATE</a> PRODUCTS, <a href="#">TALK</a> TO PEOPLE AND <a href="#" id="procrastinate">PROCRASTINATE</a>!</p>
		<p class="like"><a href="#">FOLLOW ME ELSEWHERE</a><p>
	</div>
</div>



<!-- Arrows Bottom -->




	<div class="arrow-container">
		<a id="arrow-top" href="#" class="arrow-top">text</a>
		<a href="#" class="arrow-left">text</a>
		<a href="#" class="arrow-bottom">text</a>
		<a href="#" class="arrow-right">text</a>
		</ul>
	</div>


<!-- Tool Tips -->

<div id="tooltip-procrastinate" class="tooltip-procrastinate">
	<img src="tip.png" class="tip" />
	<p class="title">Super Awesome Stuff</p>
	<img src="tooltip-sep.png" class="border" />
	<div class="categories">
		<ul>
			<li><a href="#">Design<span class="post-counter">100</span></a></li>
			<li><a href="#">Music<span class="post-counter">6</span></a></li>
			<li><a href="#">Life Lessons<span class="post-counter">567</span></a></li>
			<li><a href="#">Whatever<span class="post-counter">34</span></a></li>
			<li><a href="#">Making<span class="post-counter">10</span></a></li>
		</ul>
	</div>
</div>



	<div id="tooltip-subscribe" class="tooltip-subscribe">
		<img src="tip.png" class="tip" />
		<p class="title">Subscribe the Updates</p>
		<img src="tooltip-sep.png" class="border" />
		facebook + twitter

	</div>


	<div id="tooltip-bottom" class="tooltip-bottom">
		<img src="tip-bottom1.png" class="tip-bottom1" />
		<img src="tip-bottom2.png" class="tip-bottom2" />
		<p class="navigate">Sit back and navigate
		with the tip of fingers</p>
	</div>

<img src="earth.jpeg" style="position: fixed; left: 80px; top: -600px; z-index: -10;"/>

</body>


</html>