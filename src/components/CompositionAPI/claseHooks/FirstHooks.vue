<template>
  <div>{{ text }}</div>
  <div>{{ obj }}</div>
</template>

<script setup>
// ref= variables reactivas

//reactive es para variables reactivas pero para objetos,
//no es necesario el value solo el nombre de la key
import { ref, reactive, onMounted } from "vue";

let text = ref("Hello Vue");

const obj = reactive({ something: "example with reactive" });

onMounted(() => {
  console.log("mounted", text.value);
  console.log(obj.something);
});
</script>
