<script setup>
import Parent from "@/components/Parent.vue";
// import {provide, ref} from "vue";
//
// const numbers = ref([1,2,3,4,5,6,7,8,9])
//
// provide("numbers", numbers)
//
// const addNumber = (num) => {
//   numbers.value.push(num)
// }
</script>

<template>
  <main>
<!--    <Parent :numbers="numbers" />-->
    <Parent />
  </main>
</template>

<style scoped>
main {
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
