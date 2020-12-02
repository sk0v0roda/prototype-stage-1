<template>
  <div class="promo-main">
    <div class="container">
      <div class="row">
        <div class="col-4" v-for="card in cards" :key="card.index">
          <div class="card border-0">
            <img
              src="..\assets\img-template.svg"
              class="card-img-top mb-3"
              alt="img"
            />
            <div class="card-body p-0">
              <h5 class="card-title">{{ card.title }}</h5>
              <div>
                <span class="badge badge-dark">Тортик</span>
                <span class="badge badge-dark">Авторучка</span>
                <span class="badge badge-dark">Канделябр</span>
              </div>
              <p class="card-text">{{ card.description }}</p>
            </div>
            <div class="card-footer border-0 p-0">
              <a href="#" class="btn btn-primary"> Купить </a>
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
export default {
  data() {
    return {
      cards: [
        {
          title: 'Торты за 50%, вы не ослышались',
          description: `Психоанализ порождает гендер. Скиннер выдвинул концепцию "оперантного",
              подкрепляемого
              научения, в которой предсознательное отталкивает потребительский системный анализ.`,
          src:
            '..\\assets\\png-transparent-cupcake-computer-icons-cake-pop-cupcake-icon-food-cake-artwork.png',
        },
        {
          title: 'У нас нет сахара вообще нет не купили забыли',
          description: `Lorem ipsum dolor sit amet, consectetur adipisicing elit. Consequatur deleniti fugit
        incidunt ipsam laudantium nemo numquam, officia omnis optio quisquam ratione tempora. At consequatur
        doloremque ducimus quis sint tenetur, vel!`,
          src:
            '..\\assets\\png-transparent-cupcake-computer-icons-cake-pop-cupcake-icon-food-cake-artwork.png',
        },
        {
          title: 'У нас нет сахара вообще нет не купили забыли',
          description: `Lorem ipsum dolor sit amet, consectetur adipisicing elit. Consequatur deleniti fugit
        incidunt ipsam laudantium nemo numquam, officia omnis optio quisquam ratione tempora. At consequatur
        doloremque ducimus quis sint tenetur, vel!`,
          src:
            '..\\assets\\png-transparent-cupcake-computer-icons-cake-pop-cupcake-icon-food-cake-artwork.png',
        },
      ],
    };
  },
};
</script>

<style scoped>
@import url('../root.css');

.buy,
.catalogue {
  background: #555bec;
  width: 100%;
  height: 64px;
  margin-left: auto;
  margin-right: auto;
  align-items: center;
  text-align: center;
}

.btn-primary {
  font-family: 'Open Sans', sans-serif;
  font-size: 20px;
  text-transform: uppercase;
  font-weight: 800;
  font-size: 20px;
  width: 100%;
  background: #555bec;
  padding: 20px 0;
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

span.badge {
  padding: 7px;
  text-transform: uppercase;
  font-size: 18px;
  margin: 4px;
  color: #333333;
  background: #c0c0c0;
}

.promo-main {
  margin: 5px;
  padding: 30px;
}
</style>