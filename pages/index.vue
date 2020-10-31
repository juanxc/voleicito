<template>
  <div class="vcontainer">
    <div>
      <h1 class="title">voleicito</h1>
      <h2 class="subtitle">Encuentra donde jugar voley</h2>
      <Cabecera />
      <div class="mt-2 col-md-12"></div>
      <Lugar />
    </div>
  </div>
</template>

<script>
import Lugar from '~/components/Lugar.vue'
import Cabecera from '~/components/Cabecera.vue'

export default {
  components: {
    Lugar,
    Cabecera
  }
}
</script>
