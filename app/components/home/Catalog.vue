<template>
  <section class="catalog">
    <div class="container">
      <div class="catalog__wrapper">
        <div class="catalog__header">
          <h2 class="catalog__title">Каталог</h2>
          <div class="catalog__navigation">
            <button class="catalog__nav-btn catalog__nav-btn--prev">
              <svg width="24" height="24" viewBox="0 0 24 24" fill="none">
                <path
                  d="M15 18L9 12L15 6"
                  stroke="currentColor"
                  stroke-width="2"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                />
              </svg>
            </button>
            <button class="catalog__nav-btn catalog__nav-btn--next">
              <svg width="24" height="24" viewBox="0 0 24 24" fill="none">
                <path
                  d="M9 18L15 12L9 6"
                  stroke="currentColor"
                  stroke-width="2"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                />
              </svg>
            </button>
          </div>
        </div>

        <div class="catalog__grid">
          <div class="catalog__card">
            <div class="catalog__card-image">
              <img
                src="/img/lazer-1.webp"
                alt="Лазерный уровень ZENIT MINI 2D"
                class="catalog__img"
              />
            </div>
            <div class="catalog__card-content">
              <h3 class="catalog__card-title">
                Профессиональный лазерный уровень ZENIT MINI 2D
              </h3>
              <p class="catalog__card-description">
                16 линий 360 градусов, зеленый луч, откалиброван, гарантия,
                пульт
              </p>
            </div>
            <div class="catalog__card-price">
              <span class="catalog__price-current">От 15 990 ₽</span>
              <NuxtLink to="/" class="catalog__card-btn">Смотреть</NuxtLink>
            </div>
          </div>

          <div class="catalog__card">
            <div class="catalog__card-image">
              <img
                src="/img/lazer-1.webp"
                alt="Лазерный уровень ZENIT MINI 2D"
                class="catalog__img"
              />
            </div>
            <div class="catalog__card-content">
              <h3 class="catalog__card-title">
                Профессиональный лазерный уровень ZENIT MINI 2D
              </h3>
              <p class="catalog__card-description">
                16 линий 360 градусов, зеленый луч, откалиброван, гарантия,
                пульт
              </p>
            </div>
            <div class="catalog__card-price">
              <span class="catalog__price-current">От 15 990 ₽</span>
              <NuxtLink to="/" class="catalog__card-btn">Смотреть</NuxtLink>
            </div>
          </div>
          <div class="catalog__card">
            <div class="catalog__card-image">
              <img
                src="/img/lazer-1.webp"
                alt="Лазерный уровень ZENIT MINI 2D"
                class="catalog__img"
              />
            </div>
            <div class="catalog__card-content">
              <h3 class="catalog__card-title">
                Профессиональный лазерный уровень ZENIT MINI 2D
              </h3>
              <p class="catalog__card-description">
                16 линий 360 градусов, зеленый луч, откалиброван, гарантия,
                пульт
              </p>
            </div>
            <div class="catalog__card-price">
              <span class="catalog__price-current">От 15 990 ₽</span>
              <NuxtLink to="/" class="catalog__card-btn">Смотреть</NuxtLink>
            </div>
          </div>
          <div class="catalog__card">
            <div class="catalog__card-image">
              <img
                src="/img/lazer-1.webp"
                alt="Лазерный уровень ZENIT MINI 2D"
                class="catalog__img"
              />
            </div>
            <div class="catalog__card-content">
              <h3 class="catalog__card-title">
                Профессиональный лазерный уровень ZENIT MINI 2D
              </h3>
              <p class="catalog__card-description">
                16 линий 360 градусов, зеленый луч, откалиброван, гарантия,
                пульт
              </p>
            </div>
            <div class="catalog__card-price">
              <span class="catalog__price-current">От 15 990 ₽</span>
              <NuxtLink to="/" class="catalog__card-btn">Смотреть</NuxtLink>
            </div>
          </div>
          <div class="catalog__card">
            <div class="catalog__card-image">
              <img
                src="/img/lazer-1.webp"
                alt="Лазерный уровень ZENIT MINI 2D"
                class="catalog__img"
              />
              <div class="catalog__badge catalog__badge--sale">-23%</div>
            </div>
            <div class="catalog__card-content">
              <h3 class="catalog__card-title">
                Профессиональный лазерный уровень ZENIT MINI 2D
              </h3>
              <p class="catalog__card-description">
                16 линий 360 градусов, зеленый луч, откалиброван, гарантия,
                пульт
              </p>
            </div>
            <div class="catalog__card-price">
              <span class="catalog__price-current">От 15 990 ₽</span>
              <NuxtLink to="/" class="catalog__card-btn">Смотреть</NuxtLink>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script lang="ts" setup></script>

<style lang="scss" scoped>
.catalog {
  background: #f8f9fa;
  padding: 80px 0;
  position: relative;
  @media screen and (max-width: 1200px) {
    padding: 60px 0;
  }
  @media screen and (max-width: 635px) {
    padding: 40px 0;
  }

  &__header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 50px;
    @media screen and (max-width: 635px) {
      margin-bottom: 20px;
    }
  }

  &__title {
    color: #000000;
    font-family: 'Onest';
    font-size: 38px;
    font-weight: 700;
    line-height: 1.2;
    margin: 0;
    background: linear-gradient(135deg, #000000, #5a9f5e);
    background-clip: text;
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    @media screen and (max-width: 1200px) {
      font-size: 30px;
    }
    @media screen and (max-width: 635px) {
      font-size: 24px;
    }
  }

  &__navigation {
    display: flex;
    gap: 10px;
  }

  &__nav-btn {
    width: 44px;
    height: 44px;
    border: 2px solid #5a9f5e;
    background: #ffffff;
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    color: #5a9f5e;
    cursor: pointer;
    transition: all 0.3s ease;

    &:hover {
      background: #5a9f5e;
      color: #ffffff;
    }
    @media screen and (max-width: 1200px) {
      width: 35px;
      height: 35px;
    }
  }

  &__grid {
    display: grid;
    grid-template-columns: repeat(5, 1fr);
    gap: 20px;
    // @media screen and (max-width: 1593px) {
    //   grid-template-columns: repeat(5, 1fr);
    // }
    @media screen and (max-width: 1123px) {
      grid-template-columns: repeat(4, 1fr);
    }
    @media screen and (max-width: 900px) {
      grid-template-columns: repeat(3, 1fr);
    }
    @media screen and (max-width: 635px) {
      grid-template-columns: repeat(2, 1fr);
    }
    @media screen and (max-width: 488px) {
      grid-template-columns: repeat(1, 1fr);
    }
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
