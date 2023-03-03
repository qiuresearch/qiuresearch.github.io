---
layout: about
title: about
permalink: /
subtitle: <i>Nucleic Acids, Genetic Medicine, Experimental Biophysics, Learning Algorithms, Science of Life</i>

profile:
  align: right
  image:
  image_circular: false # crops the image to make it circular
  address:
  
  # >
  #   <p>SEH 6510 & B2200 </p>
  #   <p>George Washington Univ.</p>
  #   <p>Washington, DC 20052</p>

news: true  # includes a list of news items
selected_papers: true # includes a list of papers marked as "selected={true}"
social: true  # includes social icons at the bottom of the page
---

<!-- Slideshow container -->
<div class="QQslideshow-container">

  <!-- Full-width images with number and caption text -->
  <div class="QQmySlides QQfadeSlide">
    <div class="QQnumbertext">1 / 5</div>
      <img src="assets/img/GW-SEH1-768x461.jpg" style="width:100%">    
    <div class="QQtext">Home@SEH</div>
  </div>

  <div class="QQmySlides QQfadeSlide">
    <div class="QQnumbertext">2 / 5</div>
      <img src="assets/img/GWU-Pegasus-768x461.png" style="width:100%">    
    <div class="QQtext">Dry Lab</div>
  </div>

  <div class="QQmySlides QQfadeSlide">
    <div class="QQnumbertext">3 / 5</div>
      <img src="assets/img/GW-SEH-B2200-768x461.png" style="width:100%">    
    <div class="QQtext">Wet Lab</div>
  </div>

  <div class="QQmySlides QQfadeSlide">
    <div class="QQnumbertext">4 / 5</div>
      <img src="assets/img/GW-SEH-B2220-xray-768x461.png" style="width:100%">    
    <div class="QQtext">Xray Lab</div>
  </div>

  <div class="QQmySlides QQfadeSlide">
    <div class="QQnumbertext">5 / 5</div>
      <img src="assets/img/GW-SEH6510-768x461.png" style="width:100%">    
    <div class="QQtext">Keyboard Lab</div>
  </div>

  <!-- Next and previous buttons -->
  <a class="QQprev" onclick="plusSlides(-1)">&#10094;</a>
  <a class="QQnext" onclick="plusSlides(1)">&#10095;</a>
</div>
<br>

<!-- The dots/circles -->
<div style="text-align:center">
  <span class="QQdot" onclick="currentSlide(1)"></span>
  <span class="QQdot" onclick="currentSlide(2)"></span>
  <span class="QQdot" onclick="currentSlide(3)"></span>
  <span class="QQdot" onclick="currentSlide(4)"></span>
  <span class="QQdot" onclick="currentSlide(5)"></span>
</div>

We are a team of like-minded explorers exploiting collective methods of physical and informational sciences to study the phenomena of life. 

On the experimental front, advanced x-ray and neutron scattering and spectroscopic approaches spearhead our efforts on measuring biomolecular structures and interactions.

On the theoretical front, we develop and test physical models to seek fundamental principles. And we embrace the emerging paradigm of data-driven discoveries through the practice of mechanistic machine learning. 

Crucially, we collaborate across disciplines to educate ourselves and inspire new ideas. Be sure to [contact us](mailto:xqiu@gwu.edu) if you are interested.

The website is under construction...

<a title="Web Analytics Made Easy - Statcounter" href="https://statcounter.com/"
target="_blank"><img class="statcounter"
src="https://c.statcounter.com/1576386/0/01235842/0/"
alt="Web Analytics Made Easy - Statcounter"
referrerPolicy="no-referrer-when-downgrade"></a>

<script>
let slideIndex = 0;
let timeout;
autoshowSlides();

function autoshowSlides() {
  // let i;
  // let slides = document.getElementsByClassName("QQmySlides");
  // for (i = 0; i < slides.length; i++) {
  //   slides[i].style.display = "none";
  // }
  slideIndex++;
  // if (slideIndex > slides.length) {slideIndex = 1}
  showSlides(slideIndex)
  // slides[slideIndex-1].style.display = "block";
  timeout = setTimeout(autoshowSlides, 4500); // Change image every 4 seconds
}

// showSlides(slideIndex);

function plusSlides(n) {
  showSlides(slideIndex += n);
}

function currentSlide(n) {
  showSlides(slideIndex = n);
}

function showSlides(n) {
  let i;
  let slides = document.getElementsByClassName("QQmySlides");
  let dots = document.getElementsByClassName("QQdot");
  if (n > slides.length) {slideIndex = 1}    
  if (n < 1) {slideIndex = slides.length}
  for (i = 0; i < slides.length; i++) {
    slides[i].style.display = "none";  
  }
  for (i = 0; i < dots.length; i++) {
    dots[i].className = dots[i].className.replace(" QQactive", "");
  }
  slides[slideIndex-1].style.display = "block";  
  dots[slideIndex-1].className += " QQactive";
  clearTimeout(timeout);
}
</script>