<template>
  <NavBar/> 
  <router-view/>
  <div class="fundal">
  <FooterCp/>
  </div>
</template>

<script>
import NavBar from './components/NavBar.vue';
import FooterCp from './components/FooterCp.vue';


export default {
  name: 'HomeView',
  components: {
    NavBar,
    FooterCp,
    
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
</style>
