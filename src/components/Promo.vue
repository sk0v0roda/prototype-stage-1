<template>
  <div class="promo-main">
    <div class="container">
      <div class="row">
        <div class="col-4" v-for="card in cards" :key="card.index">
          <div class="card" style="width: 18rem;">
            <img :src="card.img" class="card-img-top" alt="img">
            <div class="card-body">
              <h5 class="card-title">{{ card.title }}</h5>
              <span class="badge badge-dark">Тортик</span>
              <span class="badge badge-dark">Авторучка</span>
              <span class="badge badge-dark">Канделябр</span>
              <p class="card-text">{{ card.description }}</p>
              <a href="#" class="btn btn-primary buy"><span class="button-text">Купить</span></a>
            </div>
          </div>
        </div>
        <div class="col-4"></div>
        <div class="btn btn-primary catalogue col-4">В каталог</div>
      </div>
    </div>
  </div>
</template>

<script>
import tort from '../assets/png-transparent-cupcake-computer-icons-cake-pop-cupcake-icon-food-cake-artwork.png'
export default {
  data() {
    return {
      cards: [{
        title: 'Торты за 50%, вы не ослышались',
        description: `Психоанализ порождает гендер. Скиннер выдвинул концепцию "оперантного",
              подкрепляемого
              научения, в которой предсознательное отталкивает потребительский системный анализ.`,
        img: tort
      }, {
        title: 'У нас нет сахара вообще нет не купили забыли',
        description: `Lorem ipsum dolor sit amet, consectetur adipisicing elit. Consequatur deleniti fugit
        incidunt ipsam laudantium nemo numquam, officia omnis optio quisquam ratione tempora. At consequatur
        doloremque ducimus quis sint tenetur, vel!`,
        img: tort
      }, {
        title: 'У нас нет сахара вообще нет не купили забыли',
        description: `Lorem ipsum dolor sit amet, consectetur adipisicing elit. Consequatur deleniti fugit
        incidunt ipsam laudantium nemo numquam, officia omnis optio quisquam ratione tempora. At consequatur
        doloremque ducimus quis sint tenetur, vel!`,
        img: tort
      },],
    }
  }
}
</script>

<style scoped>
.buy, .catalogue {
  background: #555BEC;
  width: 100%;
  height: 64px;
  margin-left: auto;
  margin-right: auto;
  align-items: center;
  text-align: center;
}

.catalogue {
  width: 300px;
  align-self: center;
  text-transform: uppercase;
  margin: 30px;
}

.card {
  margin-top: 20px;
}

.button-text {
  font-family: 'Open-Sans';
  font-size: 20px;
  text-transform: uppercase;
}

span.badge {
  padding: 7px;
  text-transform: uppercase;
  font-size: 18px;
  margin: 4px;
  color: #333333;
  background: #C0C0C0;
}

.promo-main {
  margin: 5px;
  padding: 30px;
}
</style>