<template>
  <div class="about">
    <h1>This is an about page</h1>
    <div v-for="persona in arrayPersonas" :key="persona.id">
      <p>{{persona.nombre}}   {{persona.apellido}}</p>
    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
      arrayPersonas: [
        {
          nombre: 'pepe',
          apellido: 'gote'
        },
        {
          nombre: 'raul',
          apellido: 'traderecha'
        }
      ]
    }
  }
}
</script>
