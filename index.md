# Welcome to my website!
[Resume](https://docs.google.com/document/d/e/2PACX-1vTdXMOxjDVlwPxPEMZ2_DTfDJnAC52xALzhIjLUhGW5FnHeF41MyVcPV0RUxzgMhcjNPmRNMxvVOgRB/pub)  [Projects](project.md)  [Papers](paper.md)  [Contact](contact.md)  [Awards](awards.md)
<br>
I am Sharanya Sahu, an urban planner and spatial data scientist. <br>
<img src="image/Sharanya.JPG" alt="Sharanya Sahu Photo">

## Education
Master of City and Regional Planning from Rutgers University - New Brunswick expected 2027 <br>
BA Urban Studies, BA Data Science from UC Berkeley 2024 

## Featured Projects

<div class="carousel">
  <div class="slides">
    <div class="slide">
      <a href="batikppt.html">
        <img src="image/batik.png" alt="Slide 1">
      </a>
    </div>
    <div class="slide">
      <a href="project.html">
        <img src="image/singapore1.svg" alt="SingaporeHousingPPP">
      </a>
    </div>
    <div class = "slide">
      <a href="project.html">
        <video src="video/mapvideo.mp4" autoplay muted loop playsinline></video>
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
