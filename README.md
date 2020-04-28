# artport
artistic portfolio
<style>
			.slide-container{
			position: center;
			
			}
			.slide img{
				width:940px;
				height: 460 px;
			}
			.effect {
				animation-name:effect;
				animation-duration:1s;
			}
			@keyframes effect{
				from{
				opacity: 0.6;
				}
				to{
				opacity: 1;
				
				}
			}
			.dot-container{
				text-align:center;
				
			}
			span{
				border-radius:50%;
				height:15px;
				width:15px;
				background-color:grey;
				display:inline-block;
				transition:all 0.6s linear;
			}
			.active{
			background-color:red;
			
			}
			.photos {
			width: 220px;
			float: left;
			margin: 10px;
			height: 220px;
			}
			figure { 
			play: block;
			width: 210px;
			background-color: #9c0a00;
			height: 230px;
			margin: 0px;
			padding: 9 px;
			text-align: center;
			}
			figure img {
				width: 210px;
				height: 210px;
				
			}
		</style>
		<meta name="author" content ="Jonhy amastal">
		<meta name="keywords" content ="art, painting, artist, commissions">
		<meta name = " description" content = "Web that displays artwork of Sylvan art with the 
			ability to order commissions">
		<meta http-equiv="refresh" content= "30">
	</head>
	<title> Sylvan Art </title> 
	<body>
		<div class="slide-container">
			<div class="effect slide"> 
				<img src= "Vexxmural.jpg"height = "460px" /pg>
			</div>
			
			<div class="effect slide"> 
				<img src= "Lostera.jpg" height = "460px" /pg>
			</div>
			
			<div class="effect slide"> 
				<img src= "Oni.jpg" height = "460px" /pg>
			</div>
			
		</div>
		<div class="dot-container">
			<span></span>
			<span></span>
			<span></span>
		</div>
		
		<script>
			var index=0;
			show();
			function show() {
			var i;
			var slides=document.getElementsByClassName("slide");
			var dots=document.getElementsByTagName("span");
			for(i=0;i<slides.length;i++){
					slides[i].style.display=" none";
				}
				index=index+1;
				if(index>slides.length){
					index=1;
				}
				for(i=0;i<dots.length;i++){
				dots[i].className=dots[i].className.replace("active","");
				}
				slides[index -1].style.display="block";
				dots[index-1].className+="active";
				setTimeout(show,1500);
			}
		</script>
		
	
		<a href ="file:///C:/Users/jonhy/Documents/Web%20design/webpage%20project/bio.html" >
		<span></span>
		<span></span>
		<span></span>
		<span></span>
		Biography 
		</a>
		<a href = "https://www.instagram.com/_sylvan.art/"> 
		<span></span>
		<span></span>
		<span></span>
		<span></span>
		Gallery
		</a>
		<a href = "file:///C:/Users/jonhy/Documents/Web%20design/webpage%20project/Contact%20page%20.html"> 
		<span></span>
		<span></span>
		<span></span>
		<span></span>
		Contact
		</a>
			<a href = #> 
		<span></span>
		<span></span>
		<span></span>
		<span></span>
		Store 
		</a>
		
			<div class="photos">
				<figure><img src="Lost era.jpg" />
				<figcaption> <b> Lost Era </b></figcaption>
				</figure>
			</div>
			<div class="photos">
				<figure><img src="Fate.jpg" />
				<figcaption> <b>Fate</b> </figcaption>
				</figure>
			</div>
			<div class="photos">
				<figure><img src="oni2.jpg" />
				<figcaption> <b>Materialization</b> </figcaption>
				</figure>
			</div>
			<div class="photos">
				<figure><img src="Horus.jpg" />
				<figcaption> <b>Horus Prerogative </b></figcaption>
				</figure>
			</div>
			<div class="photos">
				<figure><img src="Voyager.jpg" />
				<figcaption> <b>Lost Voyager </b></figcaption>
				</figure>
			</div>
			<div class="photos">
				<figure><img src="Humor.jpg" />
				<figcaption> <b>Humor</b></figcaption>
				</figure>
			</div>
			<div class="photos">
				<figure><img src="Love.jpg" />
				<figcaption> <b>The Gift</b></figcaption>
				</figure>
			</div>
			<div class="photos">
				<figure><img src="Apathy.jpg" />
				<figcaption> <b>Apathy</b></figcaption>
				</figure>
			</div>
			<footer style= "padding-top:10px">
			<center><h3 style = "color:#ff0000;" >All Images are subject to copy right</h3></center>
			</footer>
	</body>
</html>
