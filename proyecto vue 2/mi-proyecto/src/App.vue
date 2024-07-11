
<script>
import Persona from './components/TablaPersonas.vue'
const name ='Vue dinamico'
</script>
const app = new Vue ({
  el: '#app' , 
  data: {
    titulo: 'Hola mundo con Vue'
  }
})


<template>
  <h1>{{titulo}}</h1>
  <Persona/>
</template>

<button type="button"
@click='cambioDeTitulo'>Cambiar Titulo</button>

<style>

</style>