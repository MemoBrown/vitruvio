<template>
  <div id="quienesSomos" class="videoContainer">
    <VueSlickCarousel v-bind="settings" class="carousel-vtrv">
      <div>
        <iframe
          src="https://www.youtube.com/embed/g6UVUvL96rE"
          frameborder="0"
          allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
          allowfullscreen
          rel="0"
          showinfo="0"
        ></iframe>
      </div>
      <div>
        <iframe
          src="https://www.youtube.com/embed/zZbjgDXJJ7k"
          frameborder="0"
          allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
          allowfullscreen
          rel="0"
          showinfo="0"
        ></iframe>
      </div>
    </VueSlickCarousel>
  </div>
</template>

<script>
import VueSlickCarousel from 'vue-slick-carousel'
import 'vue-slick-carousel/dist/vue-slick-carousel.css'
// optional style for arrows & dots
import 'vue-slick-carousel/dist/vue-slick-carousel-theme.css'

export default {
  components: { VueSlickCarousel },
  data() {
    return {
      settings: {
        arrows: true,
        dots: true,
        dotsClas: 'slick-dots custom-dot-class',
        edgeFrictio: 0.35,
        infinite: false,
        speed: 500,
        slidesToShow: 1,
        slidesToScroll: 1,
      },
    }
  },
}
</script>

<style scoped>
.videoContainer {
  text-align: center;
  width: 100%;
  height: 100vh;
  background-color: var(--metodologia);
  display: flex;
  align-items: center;
  justify-content: center;
}
.videoContainer iframe {
  border-radius: 2rem;
  width: 100rem;
  height: 60rem;
}
.carousel-vtrv {
  width: 70%;
  position: absolute;
}

/* -------------------------------------------Responsive design */

@media screen and (max-width: 1536px) {
}
@media screen and (max-width: 1440px) {
}
@media screen and (max-width: 1280px) {
  .videoContainer iframe {
    width: 80rem;
    height: 50rem;
  }
}
@media screen and (max-width: 1024px) {
  .videoContainer iframe {
    width: 70rem;
    height: 50rem;
  }
}
@media screen and (max-width: 768px) {
  .videoContainer iframe {
    width: 50rem;
    height: 30rem;
    border-radius: 1rem;
  }
}
@media screen and (max-width: 576px) {
  .videoContainer iframe {
    width: 100%;
    height: 25rem;
  }
}
@media screen and (max-width: 540px) {
}
@media screen and (max-width: 480px) {
}
@media screen and (max-width: 426px) {
  .videoContainer iframe {
    width: 100%;
    height: 20rem;
  }
}
@media screen and (max-width: 376px) {
}
@media screen and (max-width: 320px) {
  .videoContainer iframe {
    width: 100%;
    height: 15rem;
  }
}
</style>
