<template>
  <div>
    <div class="m-5 p-3">
      <h1>О нас</h1>
      <h2>Без вранья</h2>
    </div>
    <div class="container mb-5">
      <div class="row">
        <div class="col-4" v-for="card in cards" :key="card.index">
          <div class="card">
            <img :src="card.src"
                 class="card-img-top" alt="img cap">
            <div class="card-body">
              <h5 class="card-title">{{ card.heading }}</h5>
              <p class="card-text">{{ card.description }}</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      cards: [{
        heading: 'У нас нет сахара вообще нет не купили забыли',
        description: `Lorem ipsum dolor sit amet, consectetur adipisicing elit. Consequatur deleniti fugit
        incidunt ipsam laudantium nemo numquam, officia omnis optio quisquam ratione tempora. At consequatur
        doloremque ducimus quis sint tenetur, vel!`,
        src: '..\\assets\\png-transparent-cupcake-computer-icons-cake-pop-cupcake-icon-food-cake-artwork.png'
      }, {
        heading: 'У нас нет сахара вообще нет не купили забыли',
        description: `Lorem ipsum dolor sit amet, consectetur adipisicing elit. Consequatur deleniti fugit
        incidunt ipsam laudantium nemo numquam, officia omnis optio quisquam ratione tempora. At consequatur
        doloremque ducimus quis sint tenetur, vel!`,
        src: '..\\assets\\png-transparent-cupcake-computer-icons-cake-pop-cupcake-icon-food-cake-artwork.png'
      }, {
        heading: 'У нас нет сахара вообще нет не купили забыли',
        description: `Lorem ipsum dolor sit amet, consectetur adipisicing elit. Consequatur deleniti fugit
        incidunt ipsam laudantium nemo numquam, officia omnis optio quisquam ratione tempora. At consequatur
        doloremque ducimus quis sint tenetur, vel!`,
        src: '..\\assets\\png-transparent-cupcake-computer-icons-cake-pop-cupcake-icon-food-cake-artwork.png'
      },],
    }
  }
}

</script>

<style scoped>
body, .card-body {
  background-color: moccasin;
}

h1, h2 {
  text-align: center;
}

h2 {
  color: grey;
}
</style>