<script setup>
  import { ref } from 'vue';

  const contador = ref(0);

  function incrementar() {
    contador.value++;
  }

  function decrementar() {
    if (contador.value > 0) {
      contador.value--;
    }
  }

  function reiniciar() {
    contador.value = 0;
  }

</script>

<template>
  <div class="redondo">
    <h1>Contador</h1>
    <p> {{ contador }} </p>
    <button class="redondo" @click="incrementar">Incrementar</button>
    <button class="redondo" @click="decrementar">Decrementar</button>
    <button class="redondo" @click="reiniciar">Reiniciar</button>
  </div>
</template>
<style>
.redondo{
border-radius:200px;

}
</style>