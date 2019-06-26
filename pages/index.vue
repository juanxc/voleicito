<template>
  <div class="container">
    <div>
      <h1 class="title">voleicito</h1>
      <h2 class="subtitle">Encuentra donde jugar voley</h2>
      <Lugar />
    </div>
  </div>
</template>

<script>
import Lugar from '~/components/Lugar.vue'

export default {
  components: {
    Lugar
  }
}
</script>
