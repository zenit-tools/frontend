<template>
  <div>
    <section class="shurupoverty">
      <div class="container">
        <h1 class="shurupoverty__title">Товары скоро появятся в каталоге</h1>
      </div>
    </section>
  </div>
</template>

<script lang="ts" setup></script>

<style lang="scss" scoped>
.shurupoverty {
  display: flex;
  align-items: center;
  justify-content: center;
  background: #f8f9fa;
  padding: 80px 0;
  min-height: 50vh;
  @media screen and (max-width: 1200px) {
    padding: 60px 0;
  }
  @media screen and (max-width: 635px) {
    padding: 40px 0;
  }
  &__title {
    color: #000000;
    font-size: 24px;
    font-weight: 700;
    line-height: 1.2;
    margin: 0;
    @media screen and (max-width: 1200px) {
      font-size: 22px;
    }
    @media screen and (max-width: 635px) {
      font-size: 18px;
    }
  }
}
</style>
