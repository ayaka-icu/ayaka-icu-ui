<script lang="ts" setup>
import LeftLog from "./Navbars/LeftNavbar.vue";
import RightNavbar from "./Navbars/RightNavbar.vue";

</script>

<template>
  <header class="flex fixed backdrop-filter backdrop-blur-md
                 top-0 z-40 w-full flex-none transition-colors duration-300 lg:z-10
                 border-b border-gray-950/10 dark:border-gray-50/[0.2] bg-white/[0.5] dark:bg-gray-950/[0.5]"
  >
    <div class="flex-1 flex items-center justify-between max-w-screen-90 mx-auto px-4">
      <LeftLog/>
      <RightNavbar/>
    </div>
  </header>
</template>
