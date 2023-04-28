
<script>
export default {
  name: "Header"
}
</script>

<template>
  <header class="container">
    <div class="logo">
      <!-- IMG IN PERCORSO ASSOLUTO PERCHè SI TROVA IN PUBLIC -->
      <img src="/dc-logo.png" alt="Logo DC">
    </div>

    <nav>
      <ul>
        <li><a href="#">characters</a></li>
        <li><a href="#">comics</a></li>
        <li><a href="#">movies</a></li>
        <li><a href="#">tv</a></li>
        <li><a href="#">games</a></li>
        <li><a href="#">collectibles</a></li>
        <li><a href="#">video</a></li>
        <li><a href="#">fans</a></li>
        <li><a href="#">news</a></li>
        <li><a href="#">shop</a></li>
      </ul>
    </nav>
  </header>
</template>

<style lang="scss" scoped>
@use "../scss/general/mixin" as *;

header{
  
  ul{
    @include centerFlex("horizontal");
    a{
      padding: 10px;
      text-transform: uppercase;
    }
  }
}
</style>