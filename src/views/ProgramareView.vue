<template>
  <div class="fundal">
    <div class="container">
      <div class="row">
        <div class="col-md-6 pb-5">
          <h1>Spune-ne ce problemă ai, și noi avem grijă de tine!</h1>
        </div>
        <div class="col-lg-6 d-flex justify-content-center">
          <div class="alege opacity-75">
            <p>Selecteaza data</p>
            <DatePicker @fecha-seleccionada="handleFechaSeleccionada" />
          </div>
        </div>
      </div>

      <div class="row">
        <div class="col-lg-3 col-md-12 opacity-75">
          <input type="text" class="form-control" v-model="nume" placeholder="Nume" aria-label="First name">
        </div>
        <div class="col-lg-3 col-md-12 opacity-75">
          <input type="text" class="form-control" v-model="prenume" placeholder="Prenume" aria-label="Last name">
        </div>
      </div>

      <div class="row">
        <div class="col-lg-3 col-md-12 opacity-75">
          <input type="text" class="form-control" v-model="telefon" placeholder="Telefon" aria-label="First name">
        </div>
        <div class="col-lg-3 col-md-12 opacity-75">
          <select id="inputState" class="form-select">
            <option selected>Alege ora</option>
            <option>8AM-9AM</option>
            <option>9AM-10AM</option>
            <option>10AM-11AM</option>
            <option>11AM-12AM</option>
            <option>12AM-1PM</option>
            <option>1PM-2PM</option>
            <option>2PM-3PM</option>
            <option>3PM-4PM</option>
          </select>
        </div>
      </div>

      <div class="row">
        <div class="col-md-6 pb-4 opacity-75">
          <textarea class="form-control" v-model="motiv" placeholder="Motivul programării" id="floatingTextarea"></textarea>
        </div>
      </div>

      <div class="row">
        <div class="col-md-12">
          <button type="button" class="btn btn-light col-md-6" @click="CreateCity">PROGRAMEAZĂ-TE</button>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup >
import DatePicker from '../components/DatePicker.vue';
import {ref } from "vue"
import axios from "axios" 

 let id = ref(null)
 let nume = ref("")
 let prenume = ref("")
 let telefon = ref("")
//  let ora = ref("")
 let motiv = ref("")
let data = ref("")

function handleFechaSeleccionada(fecha){
     data.value = fecha
     console.log(fecha)
} 

 async function CreateCity(){
   const url = 'http://localhost:5000/submit';
  
   try{
      await axios.post(url, {
        id: id.value,
        nume: nume.value,
        prenume: prenume.value,
        telefon: telefon.value,
        ora: "esto es hora",
        motiv: motiv.value,
        data: data.value
    })
    // location.reload()
   }catch(error){
      console.log(error)
   }
  
 }


    
</script>

<style lang="scss">
.fundal {
  background-image: url(../assets/altfundal.jpg);
  background-repeat: no-repeat;
  background-size: cover;
  background-attachment: fixed;
  padding-top: 10rem;
}

.container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 15px;
}


@media (max-width: 991px) {
  .alege {
    text-align: left;
  }
}

.col-lg-6,
.col-lg-8,
.col-md-12 {
  margin-bottom: 1rem;
}
</style>
