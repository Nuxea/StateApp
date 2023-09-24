<script setup>
// import {inject} from "vue";

// const numbers = inject("numbers")
import useNumbers from "@/composables/useNumbers";

const { filterNum } = useNumbers()
</script>

<template>
  <div>
    <h1>Great Grand Child</h1>
    <p>{{ filterNum(7) }}</p>
  </div>
</template>

<style scoped>

</style>