<template>
  <div>
    <app-carousel/>
    <app-promo/>
    <app-about/>
    <app-order/>
  </div>
</template>

<script>
import About from './components/About.vue'
import Order from './components/Order.vue'
import Carousel from './components/Carousel.vue'
import Promo from './components/Promo.vue'

export default {
  components: {
    appAbout: About,
    appOrder: Order,
    appCarousel: Carousel,
    appPromo: Promo
  }
}
</script>
