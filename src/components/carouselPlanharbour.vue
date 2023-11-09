<script setup>
import "vue3-carousel/dist/carousel.css";
import { Carousel, Slide, Pagination, Navigation } from "vue3-carousel";
</script>

<template>
  <carousel :items-to-show="1">
    <slide v-for="slide in 1" :key="slide">
      <div class="carousel__item">
        <img
          class="carousel__image"
          src="../assets/screenshots/planharbour/planharbour-login.png"
          alt="screenshot showing login page for planharbour application"
        />
      </div>
    </slide>
    <slide v-for="slide in 1" :key="slide">
      <img
        class="carousel__image"
        src="../assets/screenshots/planharbour/planharbour-home.png"
        alt="screenshot showing logged in home page for planhabour application, 2 lessons already loaded"
      />
    </slide>
    <slide v-for="slide in 1" :key="slide">
      <img
        class="carousel__image"
        src="../assets/screenshots/planharbour/planharbour-lesson-generator.png"
        alt="screenshot showing the form to fill out to create a lesson"
      />
    </slide>
    <slide v-for="slide in 1" :key="slide">
      <img
        class="carousel__image"
        src="../assets/screenshots/planharbour/planharbour-generated.png"
        alt="screenshot showing a sampled lesson plan created upon clicking the create lesson button"
      />
    </slide>
    <slide v-for="slide in 1" :key="slide">
      <img
        class="carousel__image"
        src="../assets/screenshots/planharbour/planharbour-saved.png"
        alt="screenshot showing the other part of a sample created lesson plan featuring the options at the bottom- save lesson, export to pdf or resubmit any changes "
      />
    </slide>

    <template #addons>
      <Navigation />
      <Pagination />
    </template>
  </carousel>
</template>

<script>
export default {
  name: "carouselPlanharbour",
};
</script>
<style>
.carousel {
  width: 100%;
}
.carousel__item {
  width: 100%;
  border-radius: 8px;
  display: flex;
  justify-content: center;
  align-items: center;
}
.carousel__image {
  width: 100%;
}
.carousel__slide {
  padding: 10px;
}
</style>
