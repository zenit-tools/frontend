<template>
  <section class="header">
    <div class="container">
      <NuxtLink to="/service" class="header__nav-link"
        >Сервисный центр</NuxtLink
      >
      <div class="header__wrapper">
        <NuxtLink to="/" class="header__logo">ZENIT</NuxtLink>
        <nav class="header__nav">
          <ul class="list-reset header__nav-list">
            <li class="header__nav-item">
              <NuxtLink to="/lazernye-urovni" class="header__nav-link"
                >Лазерные уровни</NuxtLink
              >
            </li>
            <li class="header__nav-item">
              <NuxtLink to="/shurupoverty" class="header__nav-link"
                >Шуруповерты
              </NuxtLink>
            </li>
            <li class="header__nav-item">
              <NuxtLink to="/angle-grinders" class="header__nav-link"
                >Угловые шлифовальные машины
              </NuxtLink>
            </li>
          </ul>
        </nav>
        <div class="header__links">
          <div class="header__devLink">
            <img
              class="header__devLink-img"
              src="/img/phone.webp"
              alt="phone"
            />
            <a href="tel:89167121426" class="header__link"
              >+7 (916) 712-14-26</a
            >
          </div>
          <div class="header__devLink">
            <img class="header__devLink-img" src="/img/mail.webp" alt="mail" />
            <a href="mailto:info@zenit-tools.ru" class="header__link"
              >info@zenit-tools.ru</a
            >
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script lang="ts" setup></script>

<style lang="scss" scoped>
.header {
  padding: 30px 0;
  background: #000000;
  &__wrapper {
    display: flex;
    justify-content: space-between;
    align-items: center;
    @media screen and (max-width: 900px) {
      flex-direction: column;
      gap: 20px;
    }
    @media screen and (max-width: 635px) {
      gap: 10px;
    }
  }
  &__nav {
    &-list {
      display: flex;
      gap: 30px;
      @media screen and (max-width: 635px) {
        flex-direction: column;
        gap: 5px;
        align-items: center;
      }
    }

    &-item {
      position: relative;
    }

    &-link {
      color: #ffffff;
      font-family: 'Onest';
      font-size: 16px;
      font-weight: 500;
      line-height: 24px;
      text-decoration: none;
      position: relative;

      transition: all 0.3s ease;

      &::before {
        content: '';
        position: absolute;
        bottom: -4px;
        left: 0;
        width: 0;
        height: 2px;
        background: linear-gradient(90deg, #5a9f5e, #7bc87f);
        transition: width 0.3s ease;
      }

      &:hover {
        color: #7bc87f;

        &::before {
          width: 100%;
        }

        &::after {
          opacity: 1;
        }
      }
      @media screen and (max-width: 1200px) {
        font-size: 14px;
      }
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
  &__links {
    display: flex;
    flex-direction: column;
    gap: 10px;
  }
  &__link {
    color: #ffffff;
    font-family: 'Onest';
    font-size: 16px;
    font-weight: 500;
    line-height: 24px;
    text-decoration: none;
    position: relative;
    transition: all 0.3s ease;

    &::before {
      content: '';
      position: absolute;
      bottom: -4px;
      left: 0;
      width: 0;
      height: 2px;
      background: linear-gradient(90deg, #5a9f5e, #7bc87f);
      transition: width 0.3s ease;
    }

    &:hover {
      color: #7bc87f;

      &::before {
        width: 100%;
      }
    }
    @media screen and (max-width: 1200px) {
      font-size: 14px;
    }
  }

  &__devLink {
    display: flex;
    align-items: center;
    gap: 9px;
    &-img {
      width: 25px;
      height: 25px;
      @media screen and (max-width: 1200px) {
        width: 20px;
        height: 20px;
      }
    }
  }
}
</style>
