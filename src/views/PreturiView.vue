<template>
  <div class="pad">
    <div class="container p-5">
    <h1>Lista de preturi APdent</h1>
    <p>Un plan de tratament personalizat se poate realiza numai dupa o consultatie complexa, prin urmare va recomandam sa consultati specialistii APdent.</p>
    </div>
    <TarjetaPrice/>
  </div>
</template>

<script>
import TarjetaPrice from "../components/TarjetaPrice.vue"

export default {
  name: 'HomeView',
  components: {
    TarjetaPrice,
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
