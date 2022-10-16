<script setup>
// -----------------------------
//  img 資料綁定的方式(引用資源)
// -----------------------------
// v-bind:src 必須搭配 new URL(路徑), import.meta.url).href 寫相對檔案的路徑
// https://rogeraabbccdd.github.io/F2E-book/views/ch23.html#%E5%BC%95%E7%94%A8%E8%B3%87%E6%BA%90
import { ref } from 'vue'
const img = ref(new URL('../assets/logo2.png', import.meta.url).href)

</script>

<template>
  <div id="top-image">.
    <!-- <img src="../assets/logo2.png" alt=""> -->
    <!-- img 資料綁定的方式 -->
    <img :src="img" alt="logo">
  </div>

</template>

<style scoped>
</style>
