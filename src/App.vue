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
  <div>
    <h1>Contador</h1>
    <p> {{ contador }} </p>
    <button @click="incrementar">+</button>
    <button @click="decrementar">-</button>
    <button @click="reiniciar">Reiniciar</button>
  </div>
</template>
