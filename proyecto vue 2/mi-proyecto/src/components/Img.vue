<template>
<tabla-personas :personas="personas"
@cambioTitulo="cambiarTitulo($event)" />
</template>
<script>
export default{
    name: 'app',
    components: {
        TablaPersonas,
    },
    data(){
        return{
            //A>qui ingresamos el array de objectos
        personas[
    {
        id:1, 
        nombre: 'Thomas',
        apellido: 'Love',
    },
    {
        id:2,
        nombre: 'James',
        apellido: 'Rodrigues',
    },
{
    id: 3, 
    nombre: 'Ramilus',
    apellido: 'Gued'
},
],
        }
       },
    }
methods: {
    cambiarTitulo(contenido) {
   document.getElementsByTagName("h1") [0].textContent=contenido
    }
},
</script>