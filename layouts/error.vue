<template>
  <div class="error-page">
    <h1>Error {{ error.statusCode }}</h1>
    <p>{{ error.message }}</p>
    <nuxt-link to="/">Go back to home</nuxt-link>
  </div>
</template>

<script>
export default {
  props: {
    error: {
      type: Object,
      default: () => ({ statusCode: 500, message: 'An error occurred' }),
    },
  },
}
</script>

<style scoped>
.error-page {
  text-align: center;
  margin-top: 50px;
}
</style>
