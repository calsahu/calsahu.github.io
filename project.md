# Projects

<div class="top-nav">
  <a href="index.html">About Me</a>
  <a href="https://docs.google.com/document/d/e/2PACX-1vTdXMOxjDVlwPxPEMZ2_DTfDJnAC52xALzhIjLUhGW5FnHeF41MyVcPV0RUxzgMhcjNPmRNMxvVOgRB/pub">Resume</a>
  <a href="paper.html">Papers</a>
  <a href="awards.html">Awards</a>
  <a href="contact.html">Contact</a>
</div>

<style>
.top-nav {
  margin: 10px 0 18px;
}

.top-nav a {
  display: inline-block;
  padding: 8px 14px;
  margin-right: 8px;
  border-radius: 20px;
  background: #f2f2f2;
  font-weight: 600;
  text-decoration: none;
}

.top-nav a:hover {
  background: #e0e0e0;
}
</style>

## Maps
### Click Arrows to Navigate!

Here are some of the maps I have made. As you scroll, you can click on each map to learn more. 

<div class="carousel">
  <div class="slides">
    <div class = "slide">
      <a href="https://calsahu.github.io/faith-based-housing/">
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
        <img src="image/delhigw.png" alt="Delhi groundwater map">
      </a>
    </div>
    <div class="slide">
      <a href="https://arcg.is/4e4Gq3" target="_blank">
        <img src="image/Land Cover Change_Doral.png" alt="Doral, Florida Land Cover Change">
      </a>
    </div>
    <div class="slide">
      <a href="https://storymaps.arcgis.com/stories/3b1d5d86a54442b793bc22aff1fa5fd9" target="_blank">
        <img src="image/la188.png" alt="SF Forestry Raster Analysis">
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
document.querySelectorAll(".carousel").forEach(carousel => {

  const track = carousel.querySelector(".slides");
  const slides = carousel.querySelectorAll(".slide");
  let index = 0;

  function showSlide(i) {
    index = (i + slides.length) % slides.length;
    track.style.transform = `translateX(-${index * 100}%)`;
  }

  carousel.querySelector(".next").onclick = () => showSlide(index + 1);
  carousel.querySelector(".prev").onclick = () => showSlide(index - 1);

});
</script>

Map projects:
- [Faith-based Housing](fbhousing.md)
- [Squirrel Census Visualization](https://calsahu.github.io/CommandLineGIS/)
- [Rent-burden in San Francisco](SFrentburden.md)
- [Bhubhaneswar Map](EPICBBSR.md)
- [Delhi Groundwater Scenario](GWDelhi.md)
- [Land Use Change in Doral, Florida](https://arcg.is/4e4Gq3)
- [Urban Forestry to Combat Pollution in San Francisco School Zones](https://storymaps.arcgis.com/stories/3b1d5d86a54442b793bc22aff1fa5fd9) 





## Data Analysis
### Click Arrows to Navigate!
<div class="carousel">
  <div class="slides">
    <div class = "slide">
      <a href="cchousing.html">
        <img src="image/projA1Data100.png" alt="Wealthy neighborhoods and Sale Price">
      </a>
    </div>
    <div class="slide">
      <a href="sftranspo.html">
        <img src="image/munilyft.png" alt="Comparison on Muni and Lyft prices">
      </a>
    </div>
    <div class="slide">
      <a href="gee_lulc.html">
        <img src="image/gee_bbsr.png" alt="Google Earth Engine LULC">
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
document.querySelectorAll(".carousel").forEach(carousel => {

  const track = carousel.querySelector(".slides");
  const slides = carousel.querySelectorAll(".slide");
  let index = 0;

  function showSlide(i) {
    index = (i + slides.length) % slides.length;
    track.style.transform = `translateX(-${index * 100}%)`;
  }

  carousel.querySelector(".next").onclick = () => showSlide(index + 1);
  carousel.querySelector(".prev").onclick = () => showSlide(index - 1);

});
</script>

Data analysis projects:
- [Cook County Housing Analysis](cchousing.md)
- [Assignment researching impact of ridesharing on public transportation in San Francisco](sftranspo.md)
- [Land Use Land Cover Classifier created for Bhubaneswar](gee_lulc.md)




## Presentations
### Click Arrows to Navigate!
<div class="carousel">
  <div class="slides">
    <div class="slide">
      <a href="https://docs.google.com/presentation/d/e/2PACX-1vRyHdynAAIsFmzL-_fXcwX4Xq7MC3sf-y63_sA6qIt2kG9CEoo2BLSU0A3chcpHI0d3OmeAAH8jex-j/pub?start=false&loop=false&delayms=3000" target="_blank">
        <img src="image/singapore1.svg" alt="SingaporeHousingPPP">
      </a>
    </div>
    <div class="slide">
      <a href="memo_delhitransport.html">
        <img src="image/delhipinkpass.png" alt="Delhi Pink Pass Scheme">
      </a>
    </div>
    <div class="slide">
      <a href="batikppt.html">
        <img src="image/batik.png" alt="Batik Industry">
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
document.querySelectorAll(".carousel").forEach(carousel => {

  const track = carousel.querySelector(".slides");
  const slides = carousel.querySelectorAll(".slide");
  let index = 0;

  function showSlide(i) {
    index = (i + slides.length) % slides.length;
    track.style.transform = `translateX(-${index * 100}%)`;
  }

  carousel.querySelector(".next").onclick = () => showSlide(index + 1);
  carousel.querySelector(".prev").onclick = () => showSlide(index - 1);

});
</script>

Presentations:
- [Case Study of Singapore Public Housing](https://docs.google.com/presentation/d/e/2PACX-1vRyHdynAAIsFmzL-_fXcwX4Xq7MC3sf-y63_sA6qIt2kG9CEoo2BLSU0A3chcpHI0d3OmeAAH8jex-j/pub?start=false&loop=false&delayms=3000)
- [Delhi's Pink Pass Bus Subsidy for Women](memo_delhitransport.md)
- [How Indonesia Revived its Batik Industry](batikppt.md)



<br>

Thank you for visiting my webpage. If you are interested in collaborating, please feel free to [reach out](contact.md)! 



