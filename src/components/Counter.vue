<script setup>
import { ref } from 'vue'

const counter = ref(0)
</script>

<template>
  <section>
    <div>
      <button @click="counter--">-</button>
      <p>{{ counter }}</p>
      <button @click="counter++">+</button>
    </div>
    <div>
      <button @click="counter = 0">Reset counter</button>
    </div>
  </section>
</template>

<style scoped>
section {
  display: flex;
  flex-direction: column;
  gap: 50px;
}

section > div {
  display: flex;
  width: 300px;
  align-items: center;
  justify-content: space-evenly;
}

p {
  font-size: 55px;
}

section > div:first-child > button {
  border: none;
  font-size: 45px;
  background-color: transparent;
  font-weight: bold;
  color: #007e7a;
}

section > div:last-child > button {
  border: 1px solid #007e7a;
  font-size: 18px;
  background-color: transparent;
  color: #007e7a;
  padding: 5px 10px;
  border-radius: 10px;
}

button:hover {
  cursor: pointer;
}
</style>
