<template>
  <div>
    <Header />
    <slot />
    <Footer />
  </div>
</template>

<script lang="ts" setup></script>

<style lang="scss" scoped>
.footer {
  background-color: #000000;
}
</style>
