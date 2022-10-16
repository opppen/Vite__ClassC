<script setup>
import TopImage from '@/components/TopImage.vue'
import LeftMenu from '@/components/LeftMenu.vue'
import LeftUpdate from '@/components/LeftUpdate.vue'
import RightMarquee from '@/components/RightMarquee.vue'
import RightMain from '@/components/RightMain.vue'
import FooterName from '@/components/FooterName.vue'
</script>

<template>
  <TopImage></TopImage>
  <div id="center">
    <div id="left">
      <LeftMenu></LeftMenu>
      <LeftUpdate></LeftUpdate>
    </div>
    <div id="right">
      <RightMarquee></RightMarquee>
      <RightMain></RightMain>
    </div>
  </div>
  <FooterName></FooterName>
</template>

<style scoped>
</style>
