<template>
  <div>
    <section class="lazernye-urovni">
      <div class="container">
        <div class="lazernye-urovni__grid">
          <div class="lazernye-urovni__card">
            <div class="lazernye-urovni__card-image">
              <img
                src="/img/lazer-1.webp"
                alt="Лазерный уровень ZENIT MINI 2D"
                class="lazernye-urovni__img"
              />
            </div>
            <div class="lazernye-urovni__card-content">
              <h3 class="lazernye-urovni__card-title">
                Лазерный уровень ZENIT MINI 2D
              </h3>
              <p class="lazernye-urovni__card-description">
                ZENIT MINI 2D - это профессиональный инструмент, необходимый для
                точных измерений в строительстве и ремонте.
              </p>
            </div>
            <div class="lazernye-urovni__card-price">
              <span class="lazernye-urovni__price-current">1 990 ₽</span>
              <NuxtLink
                to="/lazernye-urovni/product-1"
                class="lazernye-urovni__card-btn"
                >Смотреть</NuxtLink
              >
            </div>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script lang="ts" setup></script>

<style lang="scss" scoped>
.lazernye-urovni {
  background: #f8f9fa;
  padding: 80px 0;

  @media screen and (max-width: 1200px) {
    padding: 60px 0;
  }
  @media screen and (max-width: 635px) {
    padding: 40px 0;
  }
  &__grid {
    display: grid;
    grid-template-columns: repeat(1, 1fr);
    gap: 20px;
  }

  &__card {
    width: 100%;
    max-width: 220px;
    background: #ffffff;
    border-radius: 20px;
    box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
    position: relative;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    @media screen and (max-width: 488px) {
      gap: 10px;
      max-width: 100%;
    }
  }

  &__card-image {
    position: relative;
    height: 250px;
    overflow: hidden;
    background: #f8f9fa;
  }

  &__img {
    width: 100%;
    max-width: 220px;
    height: 100%;
    object-fit: cover;
    object-position: top;
    @media screen and (max-width: 488px) {
      max-width: 100%;
      object-position: center;
      object-fit: contain;
    }
  }

  &__card-content {
    padding: 15px 10px;
    display: flex;
    flex-direction: column;
  }

  &__card-title {
    min-height: 50px;
    color: #000000;
    font-family: 'Onest';
    font-size: 16px;
    font-weight: 600;
    line-height: 1.3;
    margin: 0 0 12px 0;
    @media screen and (max-width: 1200px) {
      font-size: 14px;
    }
    @media screen and (max-width: 488px) {
      min-height: 1px;
    }
  }

  &__card-description {
    color: #666666;
    font-family: 'Onest';
    font-size: 14px;
    font-weight: 400;
    line-height: normal;
    margin: 0 0 20px 0;
    @media screen and (max-width: 1200px) {
      font-size: 12px;
    }
    @media screen and (max-width: 488px) {
      margin: 0 0 0px 0;
    }
  }

  &__card-price {
    margin-top: auto;
    display: flex;
    flex-direction: column;
    gap: 10px;
    padding: 10px;
  }

  &__price-current {
    color: #000000;
    font-family: 'Onest';
    font-size: 16px;
    font-weight: 700;
    line-height: 1;
    @media screen and (max-width: 1200px) {
      font-size: 14px;
    }
  }

  &__card-btn {
    background: transparent;
    color: #5a9f5e;
    border: 2px solid #5a9f5e;
    padding: 12px 24px;
    border-radius: 25px;
    font-family: 'Onest';
    font-size: 14px;
    font-weight: 600;
    line-height: 1;
    text-decoration: none;
    transition: all 0.3s ease;
    text-align: center;
    width: 100%;

    &:hover {
      background: #5a9f5e;
      color: #ffffff;
    }
    @media screen and (max-width: 1200px) {
      font-size: 12px;
      padding: 8px 10px;
    }
  }
}
</style>
