---
layout: about
title: about
permalink: /
subtitle: <i>Nucleic Acids, Genetic Medicine, Experimental Biophysics, Learning Algorithms</i>

profile:
  align: right
  image: 
  image_circular: false # crops the image to make it circular
  more_info: 
    # <p>555 your office number</p>
    # <p>123 your address street</p>
    # <p>Your City, State 12345</p>

selected_papers: false # includes a list of papers marked as "selected={true}"
social: true # includes social icons at the bottom of the page

announcements:
  enabled: true # includes a list of news items
  scrollable: true # adds a vertical scroll bar if there are more than 3 news items
  limit: 4 # leave blank to include all the news in the `_news` folder

latest_posts:
  enabled: true
  scrollable: true # adds a vertical scroll bar if there are more than 3 new posts items
  limit: 3 # leave blank to include all the blog posts
---
<style>
.QQdot {
    display: inline-block;
    width: 10px; /* Adjust size */
    height: 10px;
    background-color: black; /* Adjust color */
    border-radius: 10%; /* Makes it a circle */
    cursor: pointer; /* Optional: makes it look clickable */
    margin: 10px;
    vertical-align: middle;
}
</style>
<!-- Slideshow container -->
<div class="QQslideshow-container" style="text-align:center">

  <!-- Full-width images with number and caption text -->
  <div class="QQmySlides QQfadeSlide">
    <div class="QQnumbertext">1 / 5</div>
      <img src="assets/img/GW-SEH1-768x461.jpg" style="width:100%">    
    <div class="QQtext">Home@SEH</div>
  </div>

  <div class="QQmySlides QQfadeSlide">
    <div class="QQnumbertext">2 / 5</div>
      <img src="assets/img/GW-SEH-B2200-768x461.png" style="width:100%">    
    <div class="QQtext">Wet Lab</div>
  </div>

  <div class="QQmySlides QQfadeSlide">
    <div class="QQnumbertext">3 / 5</div>
      <img src="assets/img/GW-SEH-B2220-xray-768x461.png" style="width:100%">    
    <div class="QQtext">Xray Lab</div>
  </div>

  <div class="QQmySlides QQfadeSlide">
    <div class="QQnumbertext">4 / 5</div>
      <img src="assets/img/GWU-Pegasus-768x461.png" style="width:100%">    
    <div class="QQtext">Dry Lab</div>
  </div>

  <div class="QQmySlides QQfadeSlide">
    <div class="QQnumbertext">5 / 5</div>
      <img src="assets/img/GW-SEH6510-768x461.png" style="width:100%">    
    <div class="QQtext">Keyboard Lab</div>
  </div>

</div>

<!-- The dots/circles -->
<div style="text-align:center">
  <!-- Next and previous buttons -->
  <a class="QQprev" onclick="plusSlides(-1)">&#10094;</a>
  <span class="QQdot" onclick="currentSlide(1)"></span>
  <span class="QQdot" onclick="currentSlide(2)"></span>
  <span class="QQdot" onclick="currentSlide(3)"></span>
  <span class="QQdot" onclick="currentSlide(4)"></span>
  <span class="QQdot" onclick="currentSlide(5)"></span>
  <a class="QQnext" onclick="plusSlides(1)">&#10095;</a>
</div>

We are a team of like-minded explorers exploiting collective methods of physical and statistical sciences to study the phenomena of life. 

On the experimental front, advanced x-ray and neutron scattering and spectroscopic approaches spearhead our efforts on measuring biomolecular structures and interactions.

On the theoretical front, we develop and test physical models to seek fundamental principles. And we embrace the emerging paradigm of data-driven discoveries through the practice of mechanistic machine learning. 

Crucially, we collaborate across disciplines to educate ourselves and inspire new ideas. Be sure to [contact us](mailto:xqiu@gwu.edu) if you are interested. :smile: <a title="Web Analytics Made Easy - Statcounter" href="https://statcounter.com/"
target="_blank"><img class="statcounter"
src="https://c.statcounter.com/1576386/0/01235842/0/"
alt="Web Analytics Made Easy - Statcounter"
referrerPolicy="no-referrer-when-downgrade"></a>


<script>
let slideIndex = 0;
let slides = document.getElementsByClassName("QQmySlides");
let dots = document.getElementsByClassName("QQdot");
let timeout = setTimeout(autoshowSlides, 300);

// autoshowSlides();

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
  clearTimeout(timeout);
  timeout = setTimeout(autoshowSlides, 4500); // Change image every 4 seconds
}

function noAutoshow() {
  let i;
  clearTimeout(timeout)
  for (i = 0; i < slides.length; i++) {
    slides[i].className = slides[slideIndex-1].className.replace(" QQfadeSlide", "");  
  }  
}
// showSlides(slideIndex);

function plusSlides(n) {
  noAutoshow()
  showSlides(slideIndex += n);
}

function currentSlide(n) {
  noAutoshow()
  showSlides(slideIndex = n);
}

function showSlides(n) {
  let i;
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
}
</script>
