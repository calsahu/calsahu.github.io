
# Unpublished for now

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
