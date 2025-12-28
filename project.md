# Projects


## Maps
<div class="carousel">
  <div class="slides">
    <div class = "slide">
      <a href="fbhousing.html">
        <video src="video/mapvideo.mp4" autoplay muted loop playsinline></video>
      </a>
    </div>
    <div class="slide">
      <a href="https://calsahu.github.io/CommandLineGIS/" target="_blank">
        <img src="image/squirrel.png" alt="Squirel Census NYC">
      </a>
    </div>
    <div class="slide">
      <a href="SFrentburden.html">
        <img src="image/MAP4_Rentburden_Principles of Housing.png" alt="RentBurdenSF">
      </a>
    </div>
    <div class="slide">
      <a href="EPICBBSR.html">
        <img src="image/EPIC_BBSR_KP_2.png" alt="BBSR Map">
      </a>
    </div>
    <div class="slide">
      <a href="GWDelhi.html">
        <img src="image/EPIC_BBSR_KP_2.png" alt="Delhi groundwater map">
      </a>
    </div>
    <div>
      <a href="https://docs.google.com/document/d/e/2PACX-1vTZZ76jcULc5QDYACa4x6GH-VeB5BdaXt95-XyAUs29dgqBwKykK6fFhXcDBfyV5A/pub" target="_blank">
        <img src="image/2025, 1985 (2).png" alt="Doral, Florida Built Up">
      </a>
    </div>
  </div>

  <button class="prev">‹</button>
  <button class="next">›</button>
</div>

<style>
.carousel {
  position: relative;
  width: 700px;
  max-width: 95%;
  margin: 1.5rem auto;
  overflow: hidden;
  border-radius: 12px;
}

.slides {
  display: flex;
  transition: transform .4s ease-in-out;
}

.slide a {
  display: block;
  height: 100%;
  width: 100%;
  text-decoration: none;
}

.slide {
  min-width: 100%;
}

.slide img,
.slide video {
  width: 100%;
  height: 600px;   /* pick any fixed height you like */
  object-fit: cover;
  display: block;
}

/* buttons */
button.prev,
button.next {
  position: absolute;
  top: 50%;
  transform: translateY(-50%);
  border: none;
  background: rgba(0,0,0,.45);
  color: #fff;
  font-size: 2.2rem;
  padding: .25rem .7rem;
  border-radius: 8px;
  cursor: pointer;
}

.prev { left: 10px; }
.next { right: 10px; }

button:hover {
  background: rgba(0,0,0,.65);
}
</style>

<script>
const slides = document.querySelectorAll(".slide");
const track = document.querySelector(".slides");
let index = 0;

function showSlide(i) {
  index = (i + slides.length) % slides.length;
  track.style.transform = `translateX(-${index * 100}%)`;
}

document.querySelector(".next").onclick = () => showSlide(index + 1);
document.querySelector(".prev").onclick = () => showSlide(index - 1);
</script>






## Data Analysis
<div class="carousel">
  <div class="slides">
    <div class = "slide">
      <a href="fbhousing.html">
        <video src="video/mapvideo.mp4" autoplay muted loop playsinline></video>
      </a>
    </div>
    <div class="slide">
      <a href="batikppt.html">
        <img src="image/batik.png" alt="Slide 1">
      </a>
    </div>
    <div class="slide">
      <a href="https://docs.google.com/presentation/d/e/2PACX-1vRyHdynAAIsFmzL-_fXcwX4Xq7MC3sf-y63_sA6qIt2kG9CEoo2BLSU0A3chcpHI0d3OmeAAH8jex-j/pub?start=false&loop=false&delayms=3000" target="_blank">
        <img src="image/singapore1.svg" alt="SingaporeHousingPPP">
      </a>
    </div>
  </div>

  <button class="prev">‹</button>
  <button class="next">›</button>
</div>

<style>
.carousel {
  position: relative;
  width: 700px;
  max-width: 95%;
  margin: 1.5rem auto;
  overflow: hidden;
  border-radius: 12px;
}

.slides {
  display: flex;
  transition: transform .4s ease-in-out;
}

.slide a {
  display: block;
  height: 100%;
  width: 100%;
  text-decoration: none;
}

.slide {
  min-width: 100%;
}

.slide img,
.slide video {
  width: 100%;
  height: 400px;   /* pick any fixed height you like */
  object-fit: cover;
  display: block;
}

/* buttons */
button.prev,
button.next {
  position: absolute;
  top: 50%;
  transform: translateY(-50%);
  border: none;
  background: rgba(0,0,0,.45);
  color: #fff;
  font-size: 2.2rem;
  padding: .25rem .7rem;
  border-radius: 8px;
  cursor: pointer;
}

.prev { left: 10px; }
.next { right: 10px; }

button:hover {
  background: rgba(0,0,0,.65);
}
</style>

<script>
const slides = document.querySelectorAll(".slide");
const track = document.querySelector(".slides");
let index = 0;

function showSlide(i) {
  index = (i + slides.length) % slides.length;
  track.style.transform = `translateX(-${index * 100}%)`;
}

document.querySelector(".next").onclick = () => showSlide(index + 1);
document.querySelector(".prev").onclick = () => showSlide(index - 1);
</script>






## Presentations
include HT memo
NITI Aayog work
Class presentations
<div class="carousel">
  <div class="slides">
    <div class="slide">
      <a href="batikppt.html">
        <img src="image/batik.png" alt="Slide 1">
      </a>
    </div>
    <div class="slide">
      <a href="https://docs.google.com/presentation/d/e/2PACX-1vRyHdynAAIsFmzL-_fXcwX4Xq7MC3sf-y63_sA6qIt2kG9CEoo2BLSU0A3chcpHI0d3OmeAAH8jex-j/pub?start=false&loop=false&delayms=3000" target="_blank">
        <img src="image/singapore1.svg" alt="SingaporeHousingPPP">
      </a>
    </div>
  </div>

  <button class="prev">‹</button>
  <button class="next">›</button>
</div>

<style>
.carousel {
  position: relative;
  width: 700px;
  max-width: 95%;
  margin: 1.5rem auto;
  overflow: hidden;
  border-radius: 12px;
}

.slides {
  display: flex;
  transition: transform .4s ease-in-out;
}

.slide a {
  display: block;
  height: 100%;
  width: 100%;
  text-decoration: none;
}

.slide {
  min-width: 100%;
}

.slide img,
.slide video {
  width: 100%;
  height: 400px;   /* pick any fixed height you like */
  object-fit: cover;
  display: block;
}

/* buttons */
button.prev,
button.next {
  position: absolute;
  top: 50%;
  transform: translateY(-50%);
  border: none;
  background: rgba(0,0,0,.45);
  color: #fff;
  font-size: 2.2rem;
  padding: .25rem .7rem;
  border-radius: 8px;
  cursor: pointer;
}

.prev { left: 10px; }
.next { right: 10px; }

button:hover {
  background: rgba(0,0,0,.65);
}
</style>

<script>
const slides = document.querySelectorAll(".slide");
const track = document.querySelector(".slides");
let index = 0;

function showSlide(i) {
  index = (i + slides.length) % slides.length;
  track.style.transform = `translateX(-${index * 100}%)`;
}

document.querySelector(".next").onclick = () => showSlide(index + 1);
document.querySelector(".prev").onclick = () => showSlide(index - 1);
</script>





## Graphics
NIUA work
<div class="carousel">
  <div class="slides">
    <div class="slide">
      <a href="earthday.html">
        <img src="image/2.png" alt="Earth Day image">
      </a>
    </div>
    <div class="slide">
      <a href="https://docs.google.com/presentation/d/e/2PACX-1vRyHdynAAIsFmzL-_fXcwX4Xq7MC3sf-y63_sA6qIt2kG9CEoo2BLSU0A3chcpHI0d3OmeAAH8jex-j/pub?start=false&loop=false&delayms=3000" target="_blank">
        <img src="image/singapore1.svg" alt="SingaporeHousingPPP">
      </a>
    </div>
  </div>

  <button class="prev">‹</button>
  <button class="next">›</button>
</div>

<style>
.carousel {
  position: relative;
  width: 700px;
  max-width: 95%;
  margin: 1.5rem auto;
  overflow: hidden;
  border-radius: 12px;
}

.slides {
  display: flex;
  transition: transform .4s ease-in-out;
}

.slide a {
  display: block;
  height: 100%;
  width: 100%;
  text-decoration: none;
}

.slide {
  min-width: 100%;
}

.slide img,
.slide video {
  width: 100%;
  height: 400px;   /* pick any fixed height you like */
  object-fit: cover;
  display: block;
}

/* buttons */
button.prev,
button.next {
  position: absolute;
  top: 50%;
  transform: translateY(-50%);
  border: none;
  background: rgba(0,0,0,.45);
  color: #fff;
  font-size: 2.2rem;
  padding: .25rem .7rem;
  border-radius: 8px;
  cursor: pointer;
}

.prev { left: 10px; }
.next { right: 10px; }

button:hover {
  background: rgba(0,0,0,.65);
}
</style>

<script>
const slides = document.querySelectorAll(".slide");
const track = document.querySelector(".slides");
let index = 0;

function showSlide(i) {
  index = (i + slides.length) % slides.length;
  track.style.transform = `translateX(-${index * 100}%)`;
}

document.querySelector(".next").onclick = () => showSlide(index + 1);
document.querySelector(".prev").onclick = () => showSlide(index - 1);
</script>


### Land Use Change in Doral, Florida

<img src="2025, 1985.png" alt="Doral, Florida">

<img src="image/2025, 1985 (2).png" alt="Doral, Florida Built Up">




