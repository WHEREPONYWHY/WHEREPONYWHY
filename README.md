<!Clubman-Barber-Shop>
<!HTML Group Project>
<html>
  <head>
    <title> Clubman BarberShop </title>
	<link href="image/BarberShop.jpg" rel="shortcut icon">
    <link href="image/SwirlPole.png" rel="shortcut icon">
	<link href="image/Skull.png" rel="shortcut icon">	<!For the icon on the title bar>
    <link href="image/Scissors.png" rel="shortcut icon">
	<style>
      #wrapper { display: flex; 
	    width: 100%;
      }
      header { background-color:#bf9b30   ;
      text-align: center;
      color: white;
      font-family: "Times New Roman", Georgia, Garamond, serif;
      font-size: .8em;
	    width: 100%
	    padding: 1em: 
      }
      nav { flex: 2;
      background-color: #f64d52 ;
      order: 1;
      color: white;
      font-family: "Times New Roman", Georgia, Garamond, serif;
      font-size: 1em;
      }
      main { flex: 4;
      background-color: #2a9bf4 ;
      order: 2;
      padding: 2em;
      color: white;
      font-family: "Times New Roman", Georgia, Garamond, serif;
      font-size: 1.2em;
      }
      footer { background-color: #bf9b30  ;
      color: white;
      text-align: center;
      font-family: "Times New Roman", Georgia, Garamond, serif;
      font-size: x-small;
	    width: 100%;
	    padding: 1em;
      }
     
      *{margin: 0; box-sizing: border-box;}
      <!Slideshow>
.slideshow-container {
  max-width: 1000px;
  position: relative;
  margin: auto;
}
.mySlides {
  display: none;
}
.prev, .next {
  cursor: pointer;
  position: relative;
  top: 50%;
  width: auto;
  padding: 1px;
  color: white;
  font-weight: bold;
  font-size: 18px;
  transition: 0.6s ease;
  border-radius: 0 3px 3px 0;
}
.text {
  color: #f2f2f2;
  font-size: 15px;
  padding: 8px 12px;
  position: relative;
  height: auto;
  width: 100%;
  text-align: center;
}
.dot {
  cursor: pointer;
  height: 15px;
  width: 15px;
  margin: 0 2px;
  background-color: #bbb;
  border-radius: 50%;
  display: inline-block;
  transition: background-color 0.6s ease;
}
.active, .dot:hover {
  background-color: #717171;
}
.fade {
  animation-name: fade;
  animation-duration: 1.5s;
}
@keyframes fade {
  from {opacity: .4}
  to {opacity: 1}
}
	  <!End Slideshow -source used heavily for reference https://www.w3schools.com/howto/howto_js_slideshow.asp>
    </style>
  </head>
  <!javascript for slideshow>
	<script>
let slideIndex = 1;
showSlides(slideIndex);

function currentSlide(n) {
  showSlides(slideIndex = n);
}

function showSlides(n) {
  let i;
  let slides = document.getElementsByClassName("mySlides");
  let dots = document.getElementsByClassName("dot");
  if (n > slides.length) {slideIndex = 1}
  if (n < 1) {slideIndex = slides.length}
  for (i = 0; i < slides.length; i++) {
    slides[i].style.display = "none";
  }
  for (i = 0; i < dots.length; i++) {
    dots[i].className = dots[i].className.replace(" active", "");
  }
  slides[slideIndex-1].style.display = "block";
  dots[slideIndex-1].className += " active";
}
</script>
	<!end javascript for slideshow - script from https://www.w3schools.com/howto/howto_js_slideshow.asp>
  <body>
    <header>
      Clubman's Barber Shop 
    </header>
    <div id="wrapper">
      <nav>
        <a href="OS1.html"> Our Story</a>
      </nav>
      <main>
        <!Slideshow>
		<div class="slideshow-container">

			<div class ="mySlides fade">
			<div class="numbertext">1/5</div>
			<img src="images/image1.jpg" alt="hallway mirror" style="width:100%">
			<div class="text">Hallay Mirror </div>
			</div>
			
			<div class ="mySlides fade">
			<div class="numbertext">2/5</div>
			<img src="images/image3.jpg" alt="Front Of Building" style="width:100%">
			<div class="text">Front Door </div>
			</div>
			
			<div class ="mySlides fade">
			<div class="numbertext">3/5</div>
			<img src="images/image5.jpg" alt="Waiting Room" style="width:100%">
			<div class="text">Waiting Room </div>
			</div>
			
			<div class ="mySlides fade">
			<div class="numbertext">4/5</div>
			<img src="images/image6.jpg" alt="Waiting Room 2" style="width:100%">
			<div class="text">Waiting Room Decorations </div>
			</div>
			
			<div class ="mySlides fade">
			<div class="numbertext">5/5</div>
			<img src="images/image7.jpg" alt="Waiting Room Chair" style="width:100%">
			<div class="text">Waiting Room Chair </div>
			</div>
			
			
		</div>
		<br>
		<div style="text-align:center">
			<span class="dot" onclick="currentSlide(1)"></span>
			<span class="dot" onclick="currentSlide(2)"></span>
			<span class="dot" onclick="currentSlide(3)"></span>
			<span class="dot" onclick="currentSlide(4)"></span>
			<span class="dot" onclick="currentSlide(5)"></span>
		</div>
		<!End Slideshow - source used heavily for reference https://www.w3schools.com/howto/howto_js_slideshow.asp>
		<br>
		<h5 style="text-align:center"> Click a dot above for pictures </h5>
	    </main>
    </div>
      <footer>
        &copy
      </footer>
  </body>
 </html>




