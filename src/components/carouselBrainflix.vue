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
          src="../assets/screenshots/brainflix/Brainflix-home.png"
          alt="screenshot showing brainflix home application"
        />
      </div>
    </slide>
    <slide v-for="slide in 1" :key="slide">
      <div class="carousel__item">
        <img
          class="carousel__image"
          src="../assets/screenshots/brainflix/Brainflix-upload.png"
          alt="screenshot showing brainflix upload page"
        />
      </div>
    </slide>

    <template #addons>
      <Navigation />
      <Pagination />
    </template>
  </carousel>
</template>

<script>
export default {
  name: "carouselBrainflix",
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
