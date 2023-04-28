
<script>
import {mainMenu} from "../data/menus"


export default {
  name: "Header",
  data(){
    return{
      mainMenu
    }
  }
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
        <li v-for="(link, index) in mainMenu" :key="index">
          <a :class="{'active' : link.isActive}" :href="link.href">{{link.text}}</a>
        </li>
        
      </ul>
    </nav>
  </header>
</template>

<style lang="scss" scoped>
@use "../scss/general/mixin" as *;
@use "../scss/general/variables" as *;


header{
  display: flex;
  align-items: center;
  justify-content: space-between;
  ul{
    display: flex;
    }
    a{
      color: #6c6c6c;
      text-transform: uppercase;
      padding: 15px;
      font-size: 0.8rem;
      font-weight: 600;
      &:hover,
      &.active{
        color: $primary-color;
      }
    }
  }
</style>