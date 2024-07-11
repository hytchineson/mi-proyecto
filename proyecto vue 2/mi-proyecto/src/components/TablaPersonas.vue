<template>
    <div id="component" class="container">
        <div class="row">
        <div class="col-md-12">
            <h1>Prsonas</h1>
        </div>
    </div>
    <div class="row">
        <div class="row">
            <tabla-personas
  :personas="personas"    />      
         </div>
       </div>
     </div>  
     <Img />
     <Comp />
     <button type="button"
     @click='cambioDeTitulo'>Cambiar Titulo</button>
</template>

<script>
import Img from './Img.vue'
import Compo from './component.vue'
export default{
    name: 'component',
    props{
        personas: Array
    },
    methods: {
        cambioDeTitulo(){
            this.$emit('cambioTitulo', 'Lista de personas')
        }

    }
}

</script>