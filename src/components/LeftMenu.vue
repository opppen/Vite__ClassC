<script setup>
// -----------------------------
//  img 資料綁定的方式(引用資源)
// -----------------------------
// v-bind:src 必須搭配 new URL(路徑), import.meta.url).href 寫相對檔案的路徑
// https://rogeraabbccdd.github.io/F2E-book/views/ch23.html#%E5%BC%95%E7%94%A8%E8%B3%87%E6%BA%90
import { reactive } from 'vue'
const clubs = reactive([
  '吉他', '熱舞', '棒球', '羽球', '足球', '童軍'
])

</script>

<template>
  <div id="left-menu">
    <h1>社團介紹</h1>
    <table>
      <tr v-for="club in clubs">
        <td>{{ club }}</td>
      </tr>
    </table>
  </div>

</template>

<style scoped>
</style>
