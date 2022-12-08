<template>
    <div class="py-16">
        <h2 class="text-3xl md:mt-4 md:text-6xl md:max-w-xl font-semibold md:font-bold mb-6">Our Products In MostVieweb</h2>
        <swiper
      :slidesPerView="3"
      :spaceBetween="30"
    :navigation="true"
      :modules="modules"
      class="mySwiper"
    >
      <swiper-slide>
        <img src="@/assets/slide.jpg" alt="">
      </swiper-slide>
      <swiper-slide>
        <img src="@/assets/slide.jpg" alt="">
      </swiper-slide>
      <swiper-slide>
        <img src="@/assets/slide.jpg" alt="">
      </swiper-slide>
      <swiper-slide>
        <img src="@/assets/slide.jpg" alt="">
      </swiper-slide>
      <swiper-slide>
        <img src="@/assets/slide.jpg" alt="">
      </swiper-slide>
      <swiper-slide>
        <img src="@/assets/slide.jpg" alt="">
      </swiper-slide>
      <swiper-slide>
        <img src="@/assets/slide.jpg" alt="">
      </swiper-slide>
      <swiper-slide>
        <img src="@/assets/slide.jpg" alt="">
      </swiper-slide>
      <swiper-slide>
        <img src="@/assets/slide.jpg" alt="">
      </swiper-slide>
    </swiper>
    </div>
  </template>
  <script>
  // Import Swiper Vue.js components
  import { Swiper, SwiperSlide } from "swiper/vue";
  
  // Import Swiper styles
  import "swiper/css";
  
  import "swiper/css/pagination";

  import { Pagination } from "swiper";
  
  export default {
    components: {
      Swiper,
      SwiperSlide,
    },
    setup() {
      return {
        modules: [Pagination],
      };
    },
  };
  </script>