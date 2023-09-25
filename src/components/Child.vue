<script setup>
import GrandChild from "@/components/GrandChild.vue";
import {useNumberStore} from "@/stores/numbers";

const { numbers, addNumber } = useNumberStore()
</script>

<template>
  <div>
    <h1>Child </h1>
    <div class="line"></div>
    <p>{{ numbers }}</p>
    <button @click="addNumber(4)">Add</button>
    <GrandChild />
  </div>
</template>

<style scoped>

</style>