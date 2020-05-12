---
layout: default
title: Home
permalink: /
---

<h1><strong>Welcome to my home page!</strong></h1>


<style>
* {box-sizing: border-box}
body {font-family: Verdana, sans-serif; margin:0}
.mySlides {display: none}
img {vertical-align: middle;}

/* Slideshow container */
.slideshow-container {
  max-width: 300px;
  position: relative;
  margin: auto;
}
/* Next & previous buttons */
.prev, .next {
  cursor: pointer;
  position: absolute;
  top: 50%;
  width: auto;
  padding: 16px;
  margin-top: -22px;
  color: white;
  font-weight: bold;
  font-size: 18px;
  transition: 0.6s ease;
  border-radius: 0 3px 3px 0;
}
/* Position the "next button" to the right */
.next {
  right: 0;
  border-radius: 3px 0 0 3px;
}
/* On hover, add a black background color with a little bit see-through */
.prev:hover, .next:hover {
  background-color: rgba(0,0,0,0.8);
}
/* Caption text */
.text {
  color: #f2f2f2;
  font-size: 15px;
  padding: 8px 12px;
  position: absolute;
  bottom: 8px;
  width: 100%;
  text-align: center;
}
/* Number text (1/3 etc) */
.numbertext {
  color: #f2f2f2;
  font-size: 12px;
  padding: 8px 12px;
  position: absolute;
  top: 0;
}
/* The dots/bullets/indicators */
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
/* Fading animation */
.fade {
  -webkit-animation-name: fade;
  -webkit-animation-duration: 1.5s;
  animation-name: fade;
  animation-duration: 1.5s;
}
@-webkit-keyframes fade {
  from {opacity: .4}
  to {opacity: 1}
}
@keyframes fade {
  from {opacity: .4}
  to {opacity: 1}
}
/* On smaller screens, decrease text size */
@media only screen and (max-width: 300px) {
  .prev, .next,.text {font-size: 11px}
}
</style>
<body>
<div class="slideshow-container">
<div class="mySlides fade">
  <div class="numbertext">1 / 26</div>
  <img src="/images/2014-12-18 14.02.35.jpg" style="width:75%">
  <div class="text">The gear is ready!</div>
</div>
<div class="mySlides fade">
  <div class="numbertext">2 / 26</div>
  <img src="/images/2014-12-18 16.43.55.jpg" style="width: 75%">
  <div class="text">A dolphin jumps ahead of us as we make passes across the channel with the ADCP </div>
</div>
<div class="mySlides fade">
  <div class="numbertext">3 / 26</div>
  <img src="/images/2015-03-20 08.55.32.jpg" style="width:75%">
  <div class="text">An old shrimping boat wrecked near the outlet at our sampling site Freshwater City</div>
</div>
<div class="mySlides fade">
  <div class="numbertext">4 / 26</div>
  <img src="/images/2015-06-10 11.01.18.jpg" style="width:75%">
  <div class="text">Practicing getting into our "gumby" suits while on the RV Kilo Moana headed to Station Aloha</div>
</div>
<div class="mySlides fade">
  <div class="numbertext">5 / 26</div>
  <img src="/images/2015-06-12 11.49.42.jpg" style="width:75%">
  <div class="text">Lab work aboard the RV Kilo Moana at Station Aloha</div>
</div>
<div class="mySlides fade">
  <div class="numbertext">6 / 26</div>
  <img src="/images/2015-07-30 08.14.50.jpg" style="width:75%">
  <div class="text">Dispensing media into our cultivation plates for an experiment aboard the RV Pelican in the Gulf of Mexico </div>
</div>
<div class="mySlides fade">
  <div class="numbertext">7 / 26</div>
  <img src="/images/2015-07-31 19.46.44.jpg" style="width:75%">
  <div class="text">A sunset on the Gulf of Mexico</div>
</div>
<div class="mySlides fade">
  <div class="numbertext">8 / 26</div>
  <img src="/images/2015-08-19 19.27.56.jpg" style="width:75%">
  <div class="text">The RV Pelican docked at LUMCON</div>
</div>
<div class="mySlides fade">
  <div class="numbertext">9 / 26</div>
  <img src="/images/2015-08-20 15.08.20.jpg" style="width:75%">
  <div class="text">An action shot as we tie to an old platform in the Gulf of Mexico</div>
</div>
<div class="mySlides fade">
  <div class="numbertext">10 / 26</div>
  <img src="/images/2015-08-22 17.25.11.jpg" style="width:75%">
  <div class="text">Deploying the CTD!</div>
</div>
<div class="mySlides fade">
  <div class="numbertext">11 / 26</div>
  <img src="/images/2015-08-22 19.11.09.jpg" style="width:75%">
  <div class="text">The sun setting on the box corer on the RV Pelican</div>
</div>
<a class="prev" onclick="plusSlides(-1)">&#10094;</a>
<a class="next" onclick="plusSlides(1)">&#10095;</a>
</div>
<br>
<div style="text-align:center">
  <span class="dot" onclick="currentSlide(1)"></span>
  <span class="dot" onclick="currentSlide(2)"></span>
  <span class="dot" onclick="currentSlide(3)"></span>
</div>
<script>
var slideIndex = 1;
showSlides(slideIndex);
function plusSlides(n) {
  showSlides(slideIndex += n);
}
function currentSlide(n) {
  showSlides(slideIndex = n);
}
function showSlides(n) {
  var i;
  var slides = document.getElementsByClassName("mySlides");
  var dots = document.getElementsByClassName("dot");
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
