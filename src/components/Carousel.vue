<template>
  <div>
    <div class="top-string">
      <h1>
        Наши товары
      </h1>
      <h2>
        Купите...
      </h2>
    </div>
    <div class="container">
      <div class="row-12">
        <carousel :center="true" :loop="true">

          <img src="../assets/carousel_pics/tort1.jpg" width="300" height="300">
          <img src="../assets/carousel_pics/tort2.jpg" width="300" height="300">
          <img src="../assets/carousel_pics/tort3.jpg" width="300" height="300">
          <img src="../assets/carousel_pics/tort4.jpg" width="300" height="300">
          <img src="../assets/carousel_pics/tort5.jpg" width="300" height="300">

        </carousel>
      </div>
    </div>
  </div>
</template>


<script>

import carousel from 'vue-owl-carousel'

export default {
  components: {carousel},
}

</script>
<style scoped>
img {
  padding: 30px;
}

h1, h2 {
  text-align: center;
}

h2 {
  color: grey;
}
.top-string {
  padding-top: 50px;
}

.container {
  border: 2px solid black;
  border-radius: 10px;
}
</style>