<script setup>

import {reactive, ref} from "vue";

// const red = ref(0)
// const blue = ref(0)
// const green = ref(0)

// const color = ref({
//   red: 0,
//   green: 0,
//   blue: 0
// })

const color = reactive({
  red: 0,
  green: 0,
  blue: 0
})

const randomColor = () => {
  // WITH REF
  // color.value.red = 166;
  // color.value.green = 155;
  // color.value.blue = 1;

  color.red = 166;
  color.green = 155;
  color.blue = 1;
}
</script>

<template>
  <main :style="{ backgroundColor: `rgb(${color.red}, ${color.green}, ${color.blue})`}">
    <div>
      <input v-model="color.red" type="number" placeholder="red">
      <input v-model="color.green" type="number" placeholder="green">
      <input v-model="color.blue" type="number" placeholder="blue">
      <button @click="randomColor">Random color</button>
    </div>
  </main>
</template>

<style scoped>
main {
  background-color: rgb(122, 50, 255);
  height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
}

div {
  display: flex;
  flex-direction: column;
  gap: 20px;
}

div input {
  padding: 10px;
  border: none;
  border-radius: 5px;
}
</style>
