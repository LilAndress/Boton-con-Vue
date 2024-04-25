<script setup>
import { ref } from 'Vue' ;

let count = ref(0);

function addvalue() {
    count.value++;
    console.log(count)
}
</script>


<template>
  <div @click="addvalue" class="bg-blue-500 text-white py-2 rounded hover:cursor-pointer hover:bg-blue-600 transition-colors inline-block">
    ¡Presioname!{{ count }}
  </div>

</template>