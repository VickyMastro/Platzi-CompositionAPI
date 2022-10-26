<template>
  <p>Usando computadas:</p>
  <div>{{ fullName }}</div>
</template>

<script setup>
import { ref, computed } from "vue";

const firstName = ref("Victoria");
const lastName = ref("Mastroianni");

const fullName = computed(() => {
  return `${firstName.value} ${lastName.value}`;
});
</script>
