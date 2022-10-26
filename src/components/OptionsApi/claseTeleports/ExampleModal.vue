<template>
  <div>
    <button @click="toggle">{{ msg }}</button>
    <Teleport to="body">
      <div class="modal" v-show="show">
        <h2>titulo</h2>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ab, illum
          quasi iste incidunt animi ex corporis cumque deserunt autem tempora
          ratione rem ipsum. Quasi sit iusto quidem natus, omnis quia.
        </p>
      </div>
    </Teleport>
  </div>
</template>

<script setup>
import { ref } from "vue";

let msg = ref("open modal");
let show = ref(false);

function toggle() {
  if (show.value === false) {
    show.value = !show.value;
    msg.value = "close modal";
  } else {
    show.value = !show.value;
    msg.value = "open modal";
  }
}
</script>
