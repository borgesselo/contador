<script setup>
import { ref } from "vue";

const contador = ref(0)

function incrementar() {
  contador.value++
  if (contador.value == 10) {
    alert(`aa`)
  }
}

function decrementar() {
  contador.value--
}
</script>

<template>
  <h1>Contador</h1>
  <p>Contador: {{ contador }}</p>
  <button @click="incrementar">+</button>
  <button @click="decrementar">-</button>
</template>

<style scoped>
</style>
