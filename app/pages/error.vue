<script setup lang="ts">
definePageMeta({ layout: 'page' })
useHead({ title: 'Test Page' })
const url = 'https://api.ayaka.icu/img/url'
const urlImg = ref(url)

const switchImg = () => {
  urlImg.value = `${url}?t=${new Date}`
}

</script>

<template>
  <LayoutPageWrapper :py="false">
<!--    <div class="bg-blue-500 h-[300px]"> </div>-->
    <ElButton type="primary" @click="switchImg">
      更换图片
    </ElButton>
    <img :src="urlImg" class="w-100" alt="">
    <div v-for="i in 100" :key="i">
      123123123123
    </div>
  </LayoutPageWrapper>
</template>

<style scoped>

</style>
