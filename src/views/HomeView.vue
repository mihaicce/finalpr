<template>
  <div class="pad">
    <CarouselBstrp/>
    <TarjetasIntereactivas/>

  </div>
</template>

<script>
import CarouselBstrp from '../components/CarouselBstrp.vue';
import TarjetasIntereactivas from '../components/TarjetasInteractivas.vue';

export default {
  name: 'HomeView',
  components: {
    CarouselBstrp, 
    TarjetasIntereactivas, 

}
}
</script>

<style>
.pad {
  padding-top: 10rem;
  padding-bottom: 3rem;
  padding-left: 5rem;
  padding-right: 5rem;
  background-image: url(../assets/altfundal.jpg);
  background-repeat: no-repeat;
  background-size: cover;
  background-attachment: fixed;
}
</style>
