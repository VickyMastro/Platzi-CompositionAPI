<template>
  <h1>{{ text }}</h1>
  <h2>{{ counter }}</h2>
</template>

<script setup>
import { ref, watch } from "vue";

const text = ref("Contador");
const counter = ref(0);

setInterval(() => {
  // falta ++ para que no ejecute
  counter.value;
}, 1500);

//(variable que observa, (newValue, oldValue))
watch(counter, (newValue, oldValue) => {
  console.log(`old: ${oldValue} - new: ${newValue}`);
});
</script>
