<script setup>
import { ref } from 'vue'

const contador = ref(0)
</script>

<template>
  <div>
    <button @click="contador++"></button>
    <button @click="contador--"></button>
    <p>Valor do contador: {{ contador }}</p>
  </div>
</template>

<style scoped>

</style>
