<template>
    <div>
        <input type="date" id="fecha" v-model="selectedDate" @change="emitFechaSeleccionada" />
    </div>
</template>

<script setup>
import {ref, defineEmits} from "vue"
let selectedDate = ref(new Date().toISOString().slice(0, 10))

const emitFechaSeleccionada = () => {
  const fecha = new Date(selectedDate.value)
  const fechaFormateada = fecha.toISOString().slice(0, 10).replace(/-/g, '')
  emit('fecha-seleccionada', fechaFormateada)
  console.log(fechaFormateada)
}
const emit = defineEmits(['fecha-seleccionada'])

</script>

<style>

</style>