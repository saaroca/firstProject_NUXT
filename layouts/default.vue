<template>
  <div>
    <Cabecera titulo="primer-nuxt" color="navbar navbar-light bg-primary"/>
    <nuxt />
  </div>
</template>

<script>
import Cabecera from '~/components/Cabecera.vue'
export default {
  components: {
    Cabecera,
  },
}
</script>
