
<script>

export default {
  name: "Section"
}
</script>

<template>
  <div class="blue">
    <div class="container">
      <div class="col">
        <img src="../assets/img/buy-comics-digital-comics.png" alt="">
        <span>DIGITAL COMICS</span>
      </div>

      <div class="col">
        <img src="../assets/img/buy-comics-merchandise.png" alt="">
        <span>DC MERCHANDISE</span>
      </div>

      <div class="col">
        <img src="../assets/img/buy-comics-subscriptions.png" alt="">
        <span>SUBSCRIPTION</span>
      </div>

      <div class="col">
        <img src="../assets/img/buy-comics-shop-locator.png" alt="">
        <span>COMIC SHOP LOCATOR</span>
      </div>

      <div class="col">
        <img src="../assets/img/buy-dc-power-visa.svg" alt="">
        <span>DC POWER VISA</span>
      </div>

    </div>
  </div>
</template>

<style lang="scss" scoped>
.container{ display: flex;
            padding: 50px;
  .col{
    display: flex;
    align-items: center;
  }
  img{
    width: 45px;
    padding-right: 10px;
  }
  span{
    color: white;
    font-size: 0.6rem;
    padding-right: 90px;
  }          
}
</style>