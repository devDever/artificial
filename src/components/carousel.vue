<template>
  <div class="carousel_wrapper">
    <carousel :settings="settings" :breakpoints="breakpoints">
      <template #slides>
        <slide v-for="card in newCards" :key="card">
          <img :src="card.src" alt="" />
          <h2>{{ card.title }}</h2>
          <p>{{ card.subtitle }}</p>
        </slide>
      </template>
      <template #addons>
        <pagination />
      </template>
    </carousel>
  </div>
</template>

<script>
import "vue3-carousel/dist/carousel.css";
import { Carousel, Slide, Pagination } from "vue3-carousel";
import { cards } from "../components/base";

export default {
  data: () => ({
    newCards: cards,

    settings: {
      itemsToShow: 5,
      snapAlign: "center",
    },
    breakpoints: {
      // 700px and up
      700: {
        itemsToShow: 5,
        snapAlign: "center",
      },
      // 1024 and up
      1024: {
        itemsToShow: 5,
        snapAlign: "start",
      },
    },
  }),
  components: {
    Carousel,
    Slide,
    Pagination,
  },
};
</script>

<style lang="scss">
@import "../assets/scss/_colors.scss";
.carousel_wrapper {
  background-color: $base-bg-color;
  padding-top: 100px;
}
.carousel {
  padding: 0 20px;
  position: relative;
}
.carousel__track {
  grid-gap: 20px;
  li.carousel__slide {
    border-radius: 10px;
    display: grid;
    grid-template-rows: repeat(3, 100px);
    justify-content: center;
    background: linear-gradient(
      180deg,
      rgba(255, 255, 255, 0.061) -41.9%,
      #ffffff18 115.68%
    );
    img {
      width: 30%;
    }
    h2 {
      font-size: 20px;
    }
    p {
      font-size: 14px;
    }
  }
}
</style>
