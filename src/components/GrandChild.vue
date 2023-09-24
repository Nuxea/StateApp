<script setup>
import GreatGrandChild from "@/components/GreatGrandChild.vue";
import useNumbers from "@/composables/useNumbers";

const { numbers, addNumber } = useNumbers()
</script>

<template>
  <div>
    <h1>Grand Child</h1>
    <div class="line"></div>
    {{ numbers }}
    <button @click="addNumber(4)">Add</button>
    <GreatGrandChild />
  </div>
</template>

<style scoped>

</style>