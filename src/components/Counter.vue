<script setup>
import { ref } from 'vue'

const counter = ref(0)

const increaseCounter = () => {
  counter.value++
}

const decreaseCounter = () => {
  counter.value--
}

const resetCounter = () => {
  counter.value = 0
}
</script>

<template>
  <section>
    <div>
      <button @click="decreaseCounter">-</button>
      <p>{{ counter }}</p>
      <button @click="increaseCounter">+</button>
    </div>
    <div>
      <button @click="resetCounter">Reset</button>
    </div>
  </section>
</template>
