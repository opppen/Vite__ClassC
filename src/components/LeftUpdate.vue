<script setup>
import { ref } from 'vue'
const data = ref(new Date().toLocaleDateString())
</script>

<template>
  <div id="left-update">
    {{ data }}
  </div>

</template>

<style scoped>
</style>
