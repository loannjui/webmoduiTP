<script setup>
import { ref } from 'vue'
import HelloWorld from './components/HelloWorld.vue'
const kelvin = ref(0);
const celsius = computed(() => kelvin.value - 273.15)
const fahrenheit = computed(()=> kelvin.value*1.8 -459.67)
</script>

<template>
  <HelloWorld />
</template>
