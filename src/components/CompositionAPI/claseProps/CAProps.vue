<template>
  <div>{{ props.propToRef }}</div>
  <div>{{ props.propStatic }}</div>
</template>

<script setup>
import { defineProps, useAttrs } from "vue";

const props = defineProps(["propToRef", "propStatic"]);

const attrs = useAttrs();
console.log(attrs);
</script>

<!-- 
  Props: no es necesario importar defineProps, Vue ya lo trae incorporado como una función interna.
  ejemplo que funciona(lo probe):
  
  import { useAttrs } from "vue";
  const props = defineProps(["propToRef", "propStatic"]);

  
  Context tiene estas propiedades: 
  atributos(useAttrs): son las props que no fueron declaradas pero 
  si pasadas al componente 

  emit: eventos y argumentos

  expose(defineExpose): funcion que permite "publicar" variables por ej 
  del componente para que las utilice otro componente

  slots: slots que recibe el componente
-->
