<script setup>
// import {inject} from "vue";

// const numbers = inject("numbers")
import useNumbers from "@/composables/useNumbers";
import {useNumberStore} from "@/stores/numbers";

const { numbers, doubleNumber } = useNumberStore()
const { filterNum } = useNumbers()
</script>

<template>
  <div>
    <h1>Great Grand Child {{ numbers }}</h1>
    <p>{{ doubleNumber }}</p>
    <p>{{ filterNum(7) }}</p>
  </div>
</template>

<style scoped>

</style>