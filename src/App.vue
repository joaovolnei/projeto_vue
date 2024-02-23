<script setup>
import { ref } from 'vue'

const contador = ref(0)
</script>

<template>
  <div>
    <button @click="contador++">+</button>
    <button @click="contador--">-</button>
    <p>Valor do contador: {{ contador }}</p>
  </div>
</template>

<style scoped>
button {
background-color: rgb(0, 225, 255);
color: rgb(255, 0, 0);
padding: 20px;
}
</style>

