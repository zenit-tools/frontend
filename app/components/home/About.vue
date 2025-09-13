<template>
  <section class="about">
    <div class="container">
      <div class="about__wrapper">
        <div class="about__content">
          <h2 class="about__title">О компании</h2>
          <p class="about__text">
            Мы - команда профессионалов, которые занимаются продажей и
            обслуживанием лазерных уровней, шуруповертов и угловых шлифовальных
            машин. Наша компания работает на рынке уже более 3 лет и
            зарекомендовала себя как надежный партнер.
          </p>
          <div class="about__features">
            <div class="about__feature">
              <div class="about__feature-icon">🔧</div>
              <h3 class="about__feature-title">Качественный сервис</h3>
              <p class="about__feature-text">
                Профессиональное обслуживание и ремонт инструментов
              </p>
            </div>
            <div class="about__feature">
              <div class="about__feature-icon">⚡</div>
              <h3 class="about__feature-title">Быстрая доставка</h3>
              <p class="about__feature-text">
                Доставляем заказы по всей России в кратчайшие сроки
              </p>
            </div>
            <div class="about__feature">
              <div class="about__feature-icon">🛡️</div>
              <h3 class="about__feature-title">Гарантия качества</h3>
              <p class="about__feature-text">
                Официальная гарантия на всю продукцию
              </p>
            </div>
          </div>
        </div>
        <div class="about__image"></div>
      </div>
    </div>
  </section>
</template>

<script lang="ts" setup></script>

<style lang="scss" scoped>
.about {
  background: linear-gradient(135deg, #000000 0%, #2d2d2d 70%, #000000 100%);
  padding: 80px 0;
  position: relative;
  overflow: hidden;

  &::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background: radial-gradient(
        circle at 20% 50%,
        rgba(90, 159, 94, 0.1) 0%,
        transparent 50%
      ),
      radial-gradient(
        circle at 80% 20%,
        rgba(123, 200, 127, 0.1) 0%,
        transparent 50%
      );
    pointer-events: none;
  }
  @media screen and (max-width: 1200px) {
    padding: 60px 0;
  }
  @media screen and (max-width: 635px) {
    padding: 40px 0;
  }
  &__wrapper {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 60px;
    align-items: center;
    position: relative;
    z-index: 2;
    @media screen and (max-width: 1200px) {
      grid-template-columns: 1fr;
      gap: 20px;
    }
  }

  &__content {
    display: flex;
    flex-direction: column;
    gap: 30px;
    @media screen and (max-width: 1200px) {
      gap: 20px;
    }
  }

  &__title {
    color: #ffffff;
    font-family: 'Onest';
    font-size: 38px;
    font-weight: 700;
    line-height: 1.2;
    margin: 0;
    background: linear-gradient(135deg, #ffffff, #7bc87f);
    background-clip: text;
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    text-shadow: 0 0 30px rgba(123, 200, 127, 0.3);
    @media screen and (max-width: 1200px) {
      font-size: 30px;
    }
    @media screen and (max-width: 635px) {
      font-size: 24px;
    }
  }

  &__text {
    color: #ffffff;
    font-family: 'Onest';
    font-size: 16px;
    font-weight: 400;
    line-height: 1.6;
    margin: 0;
    opacity: 0.9;
    @media screen and (max-width: 1200px) {
      font-size: 14px;
    }
  }

  &__features {
    display: grid;
    grid-template-columns: 1fr;
    gap: 25px;
    margin-top: 20px;
    @media screen and (max-width: 1200px) {
      gap: 15px;
    }
  }

  &__feature {
    display: flex;
    align-items: center;
    gap: 15px;
    padding: 20px;
    background: rgba(255, 255, 255, 0.05);
    border-radius: 12px;
    border: 1px solid rgba(123, 200, 127, 0.2);
    transition: all 0.3s ease;

    &:hover {
      background: rgba(123, 200, 127, 0.1);
      border-color: rgba(123, 200, 127, 0.4);
      transform: translateY(-2px);
    }
    @media screen and (max-width: 1200px) {
      gap: 10px;
      padding: 15px;
    }
    @media screen and (max-width: 635px) {
      flex-direction: column;
      gap: 5px;
      padding: 10px;
      align-items: center;
      text-align: center;
    }
  }

  &__feature-icon {
    font-size: 24px;
    flex-shrink: 0;
    @media screen and (max-width: 1200px) {
      font-size: 20px;
    }
  }

  &__feature-title {
    color: #7bc87f;
    font-family: 'Onest';
    font-size: 16px;
    font-weight: 600;
    line-height: 1.3;
    @media screen and (max-width: 1200px) {
      font-size: 14px;
    }
  }

  &__feature-text {
    color: #ffffff;
    font-family: 'Onest';
    font-size: 14px;
    font-weight: 400;
    line-height: 1.5;
    margin: 0;
    opacity: 0.8;
  }

  &__image {
    display: flex;
    justify-content: center;
    align-items: center;
    position: relative;
  }

  &__img {
    width: 100%;
    max-width: 500px;
    height: auto;
    border-radius: 20px;
    box-shadow: 0 20px 40px rgba(0, 0, 0, 0.3);
    transition: transform 0.3s ease;

    &:hover {
      transform: scale(1.02);
    }
    @media screen and (max-width: 1200px) {
      max-width: 300px;
    }
  }
}
</style>
