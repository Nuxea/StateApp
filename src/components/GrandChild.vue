<script setup>
import GreatGrandChild from "@/components/GreatGrandChild.vue";
import useNumbers from "@/composables/useNumbers";
import {useNumberStore} from "@/stores/numbers";

const { numbers, addNumber } = useNumbers()

const { filterNum } = useNumberStore()


</script>

<template>
  <div>
    <h1>Grand Child</h1>
    <div class="line"></div>
    {{ numbers }}
    <p>{{ filterNum(17) }}</p>
    <button @click="addNumber(4)">Add</button>
    <GreatGrandChild />
  </div>
</template>

<style scoped>

</style>