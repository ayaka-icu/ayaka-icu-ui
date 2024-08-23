<template>
  <div class="page">
    <LayoutPageNavbar class="navbar" />
    <LayoutPageContent>
      <slot />
    </LayoutPageContent>
    <LayoutPageFooter class="footer" />
  </div>
</template>
<style scoped lang="scss">
.page{
  overflow-x: hidden;
  .navbar{
    height: 64px;
    max-height: 64px;
  }
  .footer{
    height: 52px;
    @media (min-width: 768px) {
      height: 42px;
    }
  }
}
</style>