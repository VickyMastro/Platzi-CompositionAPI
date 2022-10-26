<template>hola {{ userName }}</template>

<script setup>
import { inject } from "vue";

const userName = inject("userName");
</script>

<!-- 
  - Sirve para pasar datos entre componentes de una mejor manera que con props,  
  porque pueden ser datos que pasen de hijos a padres y dps a nietos

  - los providers se pasaran a todos los hijos del componente donde se creen
-->
