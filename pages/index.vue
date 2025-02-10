<template>
  <div>
    <h2>Primer proyecto del curso con NUXT</h2>
    <input
      type="text"
      placeholder="Escribir parametro"
      class="form-control"
      v-model="id"
    />
    <div class="links">
      <nuxt-link to="/contactos" class="button--green">Contactos</nuxt-link>
      <nuxt-link to="/contactos/123" class="button--blue"
        >Contacto parametro</nuxt-link
      >
      <button class="btn btn-success" @click="enviarParametro(123)">
        Enviar parametro
      </button>
    </div>
  </div>
</template>

<script>
import Vue from 'vue'

export default {
  components: {
    Vue,
  },
  data() {
    return {
      id: '',
    }
  },
  methods: {
    enviarParametro(item) {
      this.$router.push({ path: '/contactos/' + item + ' ' + this.id })
    },
  },
}
</script>

<style>
.links {
  display: flex;
  justify-content: center;
  margin-top: 20px;
}
</style>
