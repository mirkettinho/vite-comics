
<script>
import { mainMenu, footerMenu } from '../data/menus';

export default {
  name: "Footer",
  data() {
    return{
      mainMenu,
      footerMenu
    }
  }
}
</script>

<template>
  <div class="bg">
    <footer class="">

      <div class="top container">

        <div class="col">
        <h4>DC COMICS</h4>
        <nav>
          <ul>
            <li v-for="(link, index) in footerMenu.dcComics" :key="index">
              <a :class="{'active' : link.isActive}" :href="link.href">{{link.text}}</a>
            </li>
          </ul>
          <h4>SHOP</h4>
          <ul>
            <li v-for="(link, index) in footerMenu.shop" :key="index">
              <a :class="{'active' : link.isActive}" :href="link.href">{{link.text}}</a>
            </li>
          </ul>
          
        </nav>
        </div>

        <div class="col">
        <h4>DC</h4>
        <nav>
          <ul>
            <li v-for="(link, index) in footerMenu.dc" :key="index">
              <a :class="{'active' : link.isActive}" :href="link.href">{{link.text}}</a>
            </li>
          </ul>
        </nav>
        </div>

        <div class="col">
        <h4>SITES</h4>
        <nav>
          <ul>
            <li v-for="(link, index) in footerMenu.sites" :key="index">
              <a :class="{'active' : link.isActive}" :href="link.href">{{link.text}}</a>
            </li>
          </ul>
        </nav>
        </div>

        <div class="logo-bg">
          <!-- <img src="../assets/img/dc-logo-bg.png" alt=""> -->
        </div>

      </div>

      <div class="bottom">
        <div class="container flex">

          <div class="left">
            <a href="#">SIGN-UP NOW!</a>
          </div>

          <div class="right">
            <h4>FOLLOW US</h4>
            <img src="../assets/img/footer-twitter.png" alt="">
            <img src="../assets/img/footer-youtube.png" alt="">
            <img src="../assets/img/footer-pinterest.png" alt="">
            <img src="../assets/img/footer-periscope.png" alt="">
          </div>
        </div>

      </div>
    </footer>
  </div>

</template>

<style lang="scss" scoped>

@use "../scss/general/variables" as *;


.bg{
  background-image: url(../assets/img/footer-bg.jpg);
  background-size: cover;
}
footer{
  padding-top: 1rem;
  height: 400px;

  .top{
    display: flex;
    padding-bottom: 40px;

    .col{
      width: 10%;
      h4{
        margin-bottom: 0.5rem;
        margin-top: 1rem;

        color: white;
      
      }
      li{
        a{
          font-size: 0.7rem;
          color: #6c6c6c;
          text-transform: capitalize;

        }
      }
    }
    .logo-bg{
      position: absolute;
      top: 200px;
      right: 250px;
    }
  }
  .bottom{
    
    background-color: #303030;
    height: 100px;
    padding-top: 40px;
    
    .flex{
      display: flex;
      justify-content: space-between;
    }
    a{
      color: white;
      padding: 10px;
      border: 2px solid $primary-color;
    }
    .right{
      display: flex;
      img{
        width: 30px;
        margin: 0px 10px 0px 10px;
      }
    }
  }

}
</style>