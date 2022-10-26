<template>
  <button @click="show = !show">Mostrar menu</button>
  <Transition name="fade">
    <MenuMenu v-show="show" />
  </Transition>
</template>

<script setup>
import { ref } from "vue";
import MenuMenu from "./MenuMenu.vue";

const show = ref(false);
</script>

<style scoped>
.fade-enter-from {
  opacity: 0;
}

.fade-leave-to {
  opacity: 0;
}

.fade-enter-active,
.fade-leave-active {
  transition: opacity 0.5s ease;
}
@media (min-width: 1024px) {
}
</style>
