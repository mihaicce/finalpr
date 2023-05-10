<template>
  <NavBar/> 
 
  <!-- <nav>
    <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link>
  </nav> -->
  <router-view/>
  <div class="fundal">
  <div class="pad">
    <CarouselBstrp/>
  </div>
  <FooterCp/>
</div>
</template>

<script>
import NavBar from './components/NavBar.vue';
import CarouselBstrp from './components/CarouselBstrp.vue';
import FooterCp from './components/FooterCp.vue';


export default {
  name: 'HomeView',
  components: {
    NavBar,
    FooterCp,
    CarouselBstrp
    
}
}
</script>

<style lang="scss">
.fundal {
  background-image: url(./assets/altfundal.jpg);
  background-repeat: no-repeat;
  background-size: cover;
  background-attachment: fixed;
}

.pad {
  padding-top: 10rem;
  padding-bottom: 3rem;
  padding-left: 5rem;
  padding-right: 5rem;
}
</style>
