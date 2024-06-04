<template>
  <carousel :items-to-show="1.5">
    <slide v-for="slide in 1" :key="slide" slideWidth="10">
      <img src="./img/JZA3carGFYk.jpg" width="400px" height="400px" />

    </slide>
    <slide v-for="slide in 1" :key="slide" slideWidth="10">
      <img src="./img/RPInPR54eso.jpg" width="400px" height="400px" />

    </slide>
    <slide v-for="slide in 1" :key="slide" slideWidth="10">
      <img src="./img/TUL5KP9tMao.jpg" width="400px" height="400px" />

    </slide>

    <template #addons>
      <navigation />
      <pagination />
    </template>
  </carousel>

  <carousel :items-to-show="1.5">
    <slide v-for="slide in 10" :key="slide">
      {{ slide }}
    </slide>

    <template #addons>
      <navigation />
      <pagination />
    </template>
  </carousel>
</template>

<script>
// If you are using PurgeCSS, make sure to whitelist the carousel CSS classes
import 'vue3-carousel/dist/carousel.css'
import { Carousel, Slide, Pagination, Navigation } from 'vue3-carousel'

export default {
  name: 'App',
  components: {
    Carousel,
    Slide,
    Pagination,
    Navigation,
  },
}
</script>
