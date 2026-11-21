
<script setup>
import { ref } from 'vue'

const count = ref(0)

function increase() {
  count.value++
}

function decrease() {
  count.value--
}

function reset() {
  count.value = 0
}
</script>

<template>
  <div class="container">
    <h1>شمارنده من</h1>

    <h2>{{ count }}</h2>

    <button @click="increase">افزایش +</button>
    <button @click="decrease">کاهش -</button>
    <button @click="reset">صفر کردن</button>
  </div>
</template>

<style scoped>
.container {
  text-align: center;
  margin-top: 100px;
  font-family: Arial;
}

h2 {
  font-size: 50px;
  color: green;
}

button {
  padding: 10px 20px;
  margin: 5px;
  cursor: pointer;
}
</style>
