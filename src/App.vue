<template>
  <div id="app">
    <!-- <ShowMenu /> -->
    <!-- <ExampleModal /> -->
    <!-- <FirstHooks /> -->
    <!-- <CAWatchers /> -->
    <!-- <CAComputed /> -->
    <CAProps :propToRef="msg" algo="alguito" propStatic="estatica" />
    <!-- <ProInj /> -->
  </div>
</template>

<script setup>
// import ShowMenu from "./components/OptionsApi/claseTransitions/ShowMenu.vue";
// import ExampleModal from "./components/OptionsApi/claseTeleports/ExampleModal.vue";
// import FirstHooks from "./components/CompositionAPI/claseHooks/FirstHooks.vue";
// import CAWatchers from "./components/CompositionAPI/claseWatch/CAWatchers.vue";
// import CAComputed from "./components/CompositionAPI/claseComputed/CAComputed.vue";

import CAProps from "@/components/CompositionAPI/claseProps/CAProps.vue";
const msg = "mando desde props dinamicas";

// import ProInj from "./components/CompositionAPI/claseProvide-Inject/ProInj.vue";
// import { provide } from "vue";
// //(nombre de la variable, valor (puede ser una constante o variable reactiva))
// provide("userName", "VickyMastro");
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>

<!-- virtual DOM: objeto con todos los elemnetos que hay en HTML -->
