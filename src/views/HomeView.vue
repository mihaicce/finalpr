<template>
  <div class="pad">
    <CarouselBstrp/>
    <TarjetasDescriptivas/>
    <DescripcionHome/>
    <TarjetasIntereactivas/>

  </div>
</template>

<script>
import TarjetasIntereactivas from '../components/TarjetasInteractivas.vue';
import CarouselBstrp from '../components/CarouselBstrp.vue';
import TarjetasDescriptivas from '../components/TarjetasDescriptivas.vue';
import DescripcionHome from '../components/DescripcionHome.vue';

export default {
  name: 'HomeView',
  components: {
    CarouselBstrp, 
    TarjetasIntereactivas,
    TarjetasDescriptivas,
    DescripcionHome, 

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
