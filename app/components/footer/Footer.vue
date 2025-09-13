<template>
  <section class="footer">
    <div class="container">
      <div class="footer__wrapper">
        <div class="footer__item">
          <div class="footer__item-wrapper">
            <a href="tel:89167121426" class="footer__link"
              >+7 (916) 712-14-26</a
            >
            <span class="footer__divider"></span>
            <p class="footer__text">ИНН: 502988298416, ИП Агеенко А. Д.</p>
          </div>
          <p class="footer__text">
            Московская область, г. Мытищи, ул. Коминтерна, 15A
          </p>
        </div>

        <NuxtLink href="/" class="footer__logo">ZENIT</NuxtLink>

        <img class="footer__qr" src="/img/qrcode.png" alt="footer" />
      </div>
      <span class="footer__dev">
        Разработка сайта:
        <a href="https://primedev.pro/" class="footer__dev-link" target="_blank"
          >PRIMEDEV.PRO</a
        >
      </span>
    </div>
  </section>
</template>

<script lang="ts" setup></script>

<style lang="scss" scoped>
.footer {
  padding: 80px 0;
  &__item {
    display: flex;
    flex-direction: column;
    gap: 10px;
    &-wrapper {
      display: flex;
      align-items: center;
      gap: 10px;
      @media screen and (max-width: 635px) {
        flex-direction: column;
        gap: 5px;
        align-items: center;
        text-align: center;
      }
    }
  }
  &__qr {
    width: 150px;
    height: 150px;
    @media screen and (max-width: 1200px) {
      width: 80px;
      height: 80px;
    }
  }
  &__link {
    color: #ffffff;
    font-size: 16px;
    font-weight: 400;
    line-height: 24px;
    @media screen and (max-width: 1200px) {
      font-size: 14px;
    }
  }
  &__text {
    color: #ffffff;
    font-size: 16px;
    font-weight: 400;
    line-height: 24px;
    @media screen and (max-width: 1200px) {
      font-size: 14px;
    }
    @media screen and (max-width: 635px) {
      text-align: center;
    }
  }
  &__divider {
    display: block;
    width: 2px;
    height: 15px;
    background-color: #ffffff;
    @media screen and (max-width: 635px) {
      display: none;
    }
  }
  &__logo {
    color: #ffffff;
    font-family: 'Onest';
    font-size: 28px;
    font-weight: 700;
    line-height: 1;
    letter-spacing: 2px;
    background: linear-gradient(135deg, #ffffff, #cccccc);
    background-clip: text;
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    text-shadow: 0 0 20px rgba(255, 255, 255, 0.1);
    @media screen and (max-width: 1200px) {
      font-size: 24px;
    }
  }
  &__wrapper {
    display: flex;
    justify-content: space-between;
    align-items: center;
    @media screen and (max-width: 900px) {
      flex-direction: column;
      gap: 20px;
    }
  }
  &__dev {
    display: block;
    padding-top: 20px;
    color: #ffffff;
    font-size: 14px;
    font-weight: 400;
    line-height: 1.4;
    text-align: left;
    @media screen and (max-width: 900px) {
      text-align: center;
    }
  }
  &__dev-link {
    color: #ffffff;
    font-size: 14px;
    font-weight: 400;
    line-height: 1.4;
  }
}
</style>
