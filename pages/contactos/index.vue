<template>
  <div>
    <Contactos />
    <h1>seccion de contactos</h1>
    <nuxt-link to="/">Inicio</nuxt-link>
  </div>
</template>

<script>
import Contactos from '~/layouts/contactos.vue'

export default {
  components: { Contactos },
}
</script>
