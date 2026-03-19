# Welcome to Sharanya Sahu's website!

<div class="top-nav">
  <a href="https://docs.google.com/document/d/e/2PACX-1vTdXMOxjDVlwPxPEMZ2_DTfDJnAC52xALzhIjLUhGW5FnHeF41MyVcPV0RUxzgMhcjNPmRNMxvVOgRB/pub">Resume</a>
  <a href="project.html">Projects</a>
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

<img src="image/Sharanya.JPG" alt="Sharanya Sahu Photo" width="450" align="left">
I’m Sharanya Sahu, a city planning graduate student with a background in data science and urban studies. I conduct statistical and spatial analyses and currently work on research spanning housing, community development, and technology. From building a database on faith-based affordable housing to applied research on AI and community resilience, I bridge technical insight with social context. I am versatile and curious, moving between planning, data, and communication to support decision-making that advances affordable, resilient cities.<br>

- [Rutgers Climate and Energy Fellow](https://rcei.rutgers.edu/rutgers-climate-and-energy-fellowships/)
- [Charlene Conrad Liebau Library Prize for Undergraduate Research](https://www.lib.berkeley.edu/about/news/library-prize-2024)
- [UC Berkeley Undergraduate Research Apprentice Summer Fellow](https://research.berkeley.edu/urap-researchers/sharanya-sahu/)

## Education
- Rutgers University New Brunswick (expected 2027) <b>Master of City and Regional Planning </b> 
- UC Berkeley (2024) <b>BA Urban Studies, BA Data Science</b>

## Scroll Through Featured Projects!

<div class="carousel">
  <div class="slides">
    <div class = "slide">
      <a href="https://calsahu.github.io/faith-based-housing/">
        <video src="video/mapvideo.mp4" autoplay muted loop playsinline></video>
      </a>
    </div>
    <div class="slide">
      <a href="doral.html" target="_blank">
        <img src="image/Land Cover Change_Doral.png" alt="Doral, Florida Built Up">
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

<br>
Thank you for visiting my webpage. If you are interested in collaborating, please feel free to [reach out](contact.md)!
