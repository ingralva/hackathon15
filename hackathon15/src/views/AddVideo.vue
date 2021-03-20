<template>
<div>
  <Titulo
    titulo="Agregar video"
  />
  <Formulario/>
  </div>
</template>

<script>

import Titulo from '../components/Titulo.vue'
import Formulario from '../components/Formulario.vue'

export default {
    name: 'AddVideo',
    components: { Titulo, Formulario },
}
</script>

<style>

</style>