<template>
  <NavBar/> 
  <FooterCp/>
  <!-- <nav>
    <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link>
  </nav> -->
  <router-view/>
</template>

<script>
import NavBar from './components/NavBar.vue';
import FooterCp from './components/FooterCp.vue';

export default {
  name: 'HomeView',
  components: {
    NavBar,
    FooterCp
   
  }
}
</script>

<style lang="scss">

</style>
