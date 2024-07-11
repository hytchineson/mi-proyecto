<template>
    <div id="tabla-personas">
        <table class="table">
            <thead>
                <tr>
                    <th>Nombre</th>
                    <th>Apellido</th>
                </tr>
            </thead>
            <tbody>
                <tr v-for="persona in personas" :key="persona.id">
                  <td>
              {{ persona.nombre}}
                 </td>
                 <td>
                    {{ persona.apellido}}
                 </td>

                </tr>
            </tbody>
        </table>
    </div>
</template>

<script>
export default{
    name: 'table-personas',
    props:{
        personas: Array
    },
}
</script>