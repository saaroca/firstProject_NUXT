<template>
  <div>
    <nav :class="color">
      <a class="navbar-brand" href="#">{{ titulo }}</a>
    </nav>
  </div>
</template>

<script>
export default {
  name: 'Cabecera',
  props: ['titulo', 'color'],
}
</script>
