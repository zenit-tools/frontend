<template>
  <section class="service">
    <div class="container" style="position: relative">
      <div class="service__wrapper">
        <img class="service__img" src="/img/service-1.webp" alt="service" />
        <img class="service__img-2" src="/img/service-2.webp" alt="service" />
        <div class="service__wrapper">
          <h2 class="service__title">Сервисный центр</h2>
          <p class="service__text">
            Позвоните нам
            <a class="service__text" href="tel:89167121426"
              >+7 (916) 712-14-26
            </a>
          </p>
          <a
            class="service__link"
            href="https://api.whatsapp.com/send?phone=79167121426"
            target="_blank"
            >Связаться через WhatsApp</a
          >
        </div>
      </div>
    </div>
  </section>
</template>

<script lang="ts" setup></script>

<style lang="scss" scoped>
.service {
  display: flex;
  align-items: center;
  background: linear-gradient(135deg, #000000 0%, #2d2d2d 50%, #000000 100%);
  min-height: 600px;
  padding: 80px 0;

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
    min-height: 400px;
  }
  @media screen and (max-width: 900px) {
    min-height: 200px;
  }
  @media screen and (max-width: 635px) {
    padding: 40px 0;
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
    line-height: 24px;
    @media screen and (max-width: 635px) {
      font-size: 14px;
    }
  }
  &__link {
    color: #ffffff;
    font-family: 'Onest';
    font-size: 16px;
    font-weight: 400;
    line-height: 24px;
    padding: 10px 20px;
    background-color: #5a9f5e;
    border-radius: 10px;
    text-decoration: none;
    transition: all 0.3s ease;
    &:hover {
      background-color: #7bc87f;
    }
    @media screen and (max-width: 1200px) {
      font-size: 14px;
      padding: 7px 10px;
    }
  }
  &__wrapper {
    display: flex;
    flex-direction: column;
    gap: 20px;
    align-items: center;
  }
  &__img {
    position: absolute;
    top: 50%;
    transform: translateY(-50%);
    left: -40px;
    width: 100%;
    max-width: 390px;
    object-fit: cover;
    @media screen and (max-width: 1593px) {
      left: 50px;
      max-width: 300px;
    }
    @media screen and (max-width: 1200px) {
      max-width: 190px;
    }
    @media screen and (max-width: 900px) {
      display: none;
    }
  }
  &__img-2 {
    position: absolute;
    top: 50%;
    transform: translateY(-50%);
    right: -40px;
    width: 100%;
    max-width: 330px;
    object-fit: cover;
    @media screen and (max-width: 1593px) {
      right: 50px;
      max-width: 300px;
    }
    @media screen and (max-width: 1200px) {
      max-width: 190px;
    }
    @media screen and (max-width: 900px) {
      display: none;
    }
  }
}
</style>
