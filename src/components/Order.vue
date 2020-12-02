<template>
  <div>
    <div class="m-5 p-3">
      <h1>Товары на заказ</h1>
    </div>
    <div class="container mb-5">
      <div class="row">
        <div class="col-6">
          <div class="card">
            <img src="../assets/tortik_order.jpg"
                 class="card-img-top" alt="img cap">
          </div>
        </div>
        <div class="col-6">
          <form>
            <div class="form-group">
              <label for="exampleInputName">Ваше имя:</label>
              <input type="text" class="form-control" id="exampleInputName">
            </div>
            <div class="form-group">
              <label for="exampleInputPhone">Ваш телефон:</label>
              <input type="tel" class="form-control" id="exampleInputPhone">
              <small id="phoneHelp" class="form-text text-muted">Мы не будем вам названивать. Базарим по делу!</small>
            </div>
            <button type="submit" class="btn btn-primary">Отправить</button>
          </form>
        </div>
      </div>
    </div>
  </div>
</template>


<script>
export default {}
</script>


<style scoped>
h1 {
  text-align: center;
}
</style>