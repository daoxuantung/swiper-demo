
<template>
<swiper :effect="'coverflow'" :grabCursor="true" :centeredSlides="true" :slidesPerView="'auto'" :coverflowEffect='{
  "rotate": 50,
  "stretch": 0,
  "depth": 100,
  "modifier": 1,
  "slideShadows": true
}' :pagination="true" class="mySwiper">
  <swiper-slide><img src="https://swiperjs.com/demos/images/nature-1.jpg" /></swiper-slide><swiper-slide><img src="https://swiperjs.com/demos/images/nature-2.jpg" /></swiper-slide><swiper-slide><img src="https://swiperjs.com/demos/images/nature-3.jpg" /></swiper-slide><swiper-slide><img src="https://swiperjs.com/demos/images/nature-4.jpg" /></swiper-slide><swiper-slide><img src="https://swiperjs.com/demos/images/nature-5.jpg" /></swiper-slide><swiper-slide><img src="https://swiperjs.com/demos/images/nature-6.jpg" /></swiper-slide><swiper-slide><img src="https://swiperjs.com/demos/images/nature-7.jpg" /></swiper-slide><swiper-slide><img src="https://swiperjs.com/demos/images/nature-8.jpg" /></swiper-slide><swiper-slide><img src="https://swiperjs.com/demos/images/nature-9.jpg" /></swiper-slide>
  </swiper>
</template>
<script>
// Import Swiper Vue.js components
import { Swiper, SwiperSlide } from 'swiper/vue';

// Import Swiper styles
import 'swiper/css';

import "swiper/css/effect-coverflow"
import "swiper/css/pagination"

import './style.css';


// import Swiper core and required modules
import SwiperCore, {
  EffectCoverflow,Pagination
} from 'swiper';

// install Swiper modules
SwiperCore.use([EffectCoverflow,Pagination]);


export default {
  components: {
    Swiper,
    SwiperSlide,
  },
  data() {
    return {
        
        
    };
  },
  methods: {
    
  }
  
}
</script>