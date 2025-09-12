<template>
  <section class="product">
    <div class="container">
      <nav class="breadcrumbs">
        <NuxtLink to="/" class="breadcrumbs__link">Главная</NuxtLink>
        <span class="breadcrumbs__separator">/</span>
        <NuxtLink to="/lazernye-urovni" class="breadcrumbs__link"
          >Лазерные уровни</NuxtLink
        >
        <span class="breadcrumbs__separator">/</span>
        <span class="breadcrumbs__current">ZENIT MINI 2D</span>
      </nav>

      <div class="product__wrapper">
        <div class="card">
          <Galleria
            :value="images"
            :responsiveOptions="responsiveOptions"
            :numVisible="5"
            :showIndicators="false"
            containerStyle="max-width: 400px"
            :showThumbnails="true"
            :showItemNavigators="true"
          >
            <template #item="slotProps">
              <img
                :src="slotProps.item.itemImageSrc"
                :alt="slotProps.item.alt"
                style="width: 100%"
              />
            </template>
            <!-- <template #thumbnail="slotProps">
              <img
                :src="slotProps.item.thumbnailImageSrc"
                :alt="slotProps.item.alt"
              />
            </template> -->
          </Galleria>
        </div>

        <div class="product__info-section">
          <h1 class="product__title">Лазерный уровень ZENIT MINI 2D</h1>

          <div class="product__price">
            <span class="product__price-current">1 990 ₽</span>
          </div>

          <div class="product__description">
            <p>
              Лазерный уровень ZENIT MINI 2D – это профессиональный инструмент,
              необходимый для точных измерений в строительстве и ремонте.
              Самовыравнивающийся нивелир обеспечивает надежное автоматическое
              нивелирование, что делает его идеальным помощником как для
              новичков, так и для опытных специалистов. Наша линейка 3д
              соответствует стандартам качества, а электронные компоненты
              гарантируют долговечность и точность измерения даже под большим
              углом.
            </p>
          </div>
        </div>
      </div>

      <div class="product__tabs">
        <div class="product__tabs-header">
          <button
            class="product__tab-btn"
            :class="{ 'product__tab-btn--active': activeTab === 'description' }"
            @click="activeTab = 'description'"
          >
            Описание
          </button>
          <button
            class="product__tab-btn"
            :class="{
              'product__tab-btn--active': activeTab === 'specifications',
            }"
            @click="activeTab = 'specifications'"
          >
            Характеристики
          </button>
        </div>

        <div class="product__tabs-content">
          <div v-show="activeTab === 'description'" class="product__tab-panel">
            <div class="product__details-text">
              <p>
                Лазерный уровень – это профессиональный инструмент, необходимый
                для точных измерений в строительстве и ремонте.
                Самовыравнивающийся нивелир обеспечивает надежное автоматическое
                нивелирование, что делает его идеальным помощником как для
                новичков, так и для опытных специалистов. Наша линейка 3д
                соответствует стандартам качества, а электронные компоненты
                гарантируют долговечность и точность измерения даже под большим
                углом.
              </p>
              <p>
                Устройство laser оснащено крестовидным лучом, что позволяет
                легко выравнивать поверхности и отмечать вертикальные и
                горизонтальные линии. Прибор подходит для укладки плитки,
                монтажа гипсокартона и других задач, связанных с точностью
                работы. Компактные размеры позволяют удобно использовать его в
                ограниченных пространствах.
              </p>
              <p>
                С защитой от влаги и пыли по классу IP54 этот лазерный
                инструмент способен работать в различных условиях, что особенно
                важно на стройплощадках. Прочный корпус из нейлонового пластика
                дополнен резиновыми вставками, обеспечивающими надежную защиту
                от ударов. Удобная активация функций одним нажатием кнопки
                делает использование прибора интуитивно понятным.
              </p>
              <p>
                Лазер предлагает возможность регулировки яркости луча для
                удобства работы в различных условиях освещения. Также имеется
                функция блокировки уровня, что позволяет фиксировать
                установленное положение во время работы.
              </p>
              <p>
                Дальность измерения достигает 30 метров, а высокая точность до
                ±2 мм на 5 м гарантирует безупречные результаты при выполнении
                любых строительных задач. Благодаря возможности наклонного луча
                настройки становятся еще более удобными.
              </p>
              <p>
                Лазерный уровень работает от батареек типа AA и не требует
                юстировки благодаря системе самоисправления. Инструмент имеет
                рабочий диапазон температур от -10°C до 50°C, что позволяет
                использовать его в любое время года.
              </p>
              <p>
                Комплект включает все необходимые аксессуары для комфортного
                использования: сумку для хранения и транспортировки устройства.
                Лазерный уровень ( дальномер , угломер оригинал) станет
                незаменимым маленький помощником как в домашних условиях, так и
                на профессиональных стройках.
              </p>
            </div>
          </div>

          <div
            v-show="activeTab === 'specifications'"
            class="product__tab-panel"
          >
            <div class="product__specifications-grid">
              <div class="product__spec-group">
                <h3 class="product__spec-group-title">Технические свойства</h3>
                <div class="product__spec-list">
                  <div class="product__spec-item">
                    <span class="product__spec-label">Количество лучей:</span>
                    <span class="product__spec-value">2</span>
                  </div>
                  <div class="product__spec-item">
                    <span class="product__spec-label"
                      >Дальность измерения, м:</span
                    >
                    <span class="product__spec-value">30</span>
                  </div>
                  <div class="product__spec-item">
                    <span class="product__spec-label"
                      >Погрешность измерения:</span
                    >
                    <span class="product__spec-value">±0.02 мм</span>
                  </div>
                  <div class="product__spec-item">
                    <span class="product__spec-label">Класс лазера:</span>
                    <span class="product__spec-value">2</span>
                  </div>
                  <div class="product__spec-item">
                    <span class="product__spec-label"
                      >Проецирование лучей:</span
                    >
                    <span class="product__spec-value">Линейное</span>
                  </div>
                  <div class="product__spec-item">
                    <span class="product__spec-label">Класс защиты:</span>
                    <span class="product__spec-value">IP54</span>
                  </div>
                  <div class="product__spec-item">
                    <span class="product__spec-label">Тип питания:</span>
                    <span class="product__spec-value"
                      >От батареек, От аккумулятора</span
                    >
                  </div>
                  <div class="product__spec-item">
                    <span class="product__spec-label">Цвет луча:</span>
                    <span class="product__spec-value">Зеленый</span>
                  </div>
                  <div class="product__spec-item">
                    <span class="product__spec-label">Функции:</span>
                    <span class="product__spec-value"
                      >Мин. уровень освещения, Макс. уровень освещения, Средний
                      уровень освещения</span
                    >
                  </div>
                </div>
              </div>

              <div class="product__spec-group">
                <h3 class="product__spec-group-title">Особенности</h3>
                <div class="product__spec-list">
                  <div class="product__spec-item">
                    <span class="product__spec-label">Особенности:</span>
                    <span class="product__spec-value"
                      >Автоматическое выравнивание, Индикатор неправильной
                      установки, Крепление для штатива, Магнитное
                      крепление</span
                    >
                  </div>
                </div>
              </div>

              <div class="product__spec-group">
                <h3 class="product__spec-group-title">Основные</h3>
                <div class="product__spec-list">
                  <div class="product__spec-item">
                    <span class="product__spec-label"
                      >Крепление головки к штативу:</span
                    >
                    <span class="product__spec-value">1/4"</span>
                  </div>
                </div>
              </div>

              <div class="product__spec-group">
                <h3 class="product__spec-group-title">Общие</h3>
                <div class="product__spec-list">
                  <div class="product__spec-item">
                    <span class="product__spec-label">Гарантия:</span>
                    <span class="product__spec-value">5 лет</span>
                  </div>
                </div>
              </div>

              <div class="product__spec-group">
                <h3 class="product__spec-group-title">Дополнительные</h3>
                <div class="product__spec-list">
                  <div class="product__spec-item">
                    <span class="product__spec-label">Цвет:</span>
                    <span class="product__spec-value">Зеленый, черный</span>
                  </div>
                  <div class="product__spec-item">
                    <span class="product__spec-label">Тип:</span>
                    <span class="product__spec-value"
                      >Лазерный уровень/нивелир</span
                    >
                  </div>
                  <div class="product__spec-item">
                    <span class="product__spec-label"
                      >Страна-изготовитель:</span
                    >
                    <span class="product__spec-value">Китай</span>
                  </div>
                  <div class="product__spec-item">
                    <span class="product__spec-label">Партномер:</span>
                    <span class="product__spec-value">нет</span>
                  </div>
                  <div class="product__spec-item">
                    <span class="product__spec-label">Комплектация:</span>
                    <span class="product__spec-value"
                      >Коробка; мягкий кейс; лазерный уровень; батарейки 2шт АА;
                      магнитный крепеж</span
                    >
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script lang="ts" setup>
import Galleria from 'primevue/galleria'

const images = ref([
  {
    itemImageSrc: '/img/1.webp',
    alt: 'Лазерный уровень ZENIT MINI 2D',
  },
  {
    itemImageSrc: '/img/2.webp',
    alt: 'Лазерный уровень ZENIT MINI 2D',
  },
  {
    itemImageSrc: '/img/3.webp',
    alt: 'Лазерный уровень ZENIT MINI 2D',
  },
  {
    itemImageSrc: '/img/4.webp',
    alt: 'Лазерный уровень ZENIT MINI 2D',
  },
  {
    itemImageSrc: '/img/5.webp',
    alt: 'Лазерный уровень ZENIT MINI 2D',
  },
  {
    itemImageSrc: '/img/6.webp',
    alt: 'Лазерный уровень ZENIT MINI 2D',
  },
  {
    itemImageSrc: '/img/7.webp',
    alt: 'Лазерный уровень ZENIT MINI 2D',
  },
  {
    itemImageSrc: '/img/8.webp',
    alt: 'Лазерный уровень ZENIT MINI 2D',
  },
  {
    itemImageSrc: '/img/9.webp',
    alt: 'Лазерный уровень ZENIT MINI 2D',
  },
])
const responsiveOptions = ref([
  {
    breakpoint: '1300px',
    numVisible: 4,
  },
  {
    breakpoint: '575px',
    numVisible: 1,
  },
])
const activeTab = ref('description')

useHead({
  title: 'ZENIT MINI 2D - Лазерный уровень | ZENIT',
  meta: [
    {
      name: 'description',
      content:
        'Лазерный уровень ZENIT MINI 2D - профессиональный инструмент для точных измерений в строительстве и ремонте. Самовыравнивающийся нивелир с дальностью 30м.',
    },
    {
      property: 'og:title',
      content: 'ZENIT MINI 2D - Лазерный уровень | ZENIT',
    },
    {
      property: 'og:description',
      content:
        'Лазерный уровень ZENIT MINI 2D - профессиональный инструмент для точных измерений в строительстве и ремонте.',
    },
    { property: 'og:type', content: 'product' },
    {
      property: 'og:url',
      content: 'https://zenit-tools.ru/lazernye-urovni/product-1',
    },
    { property: 'og:site_name', content: 'ZENIT' },
    { property: 'og:locale', content: 'ru_RU' },
    { name: 'robots', content: 'index, follow' },
  ],
})
</script>

<style lang="scss" scoped>
.product {
  background: #f8f9fa;
  padding: 80px 0;
  min-height: 100vh;

  @media screen and (max-width: 1200px) {
    padding: 60px 0;
  }
  @media screen and (max-width: 635px) {
    padding: 40px 0;
  }
}

.breadcrumbs {
  display: flex;
  align-items: center;
  gap: 8px;
  margin-bottom: 30px;
  font-family: 'Onest';
  font-size: 14px;
  font-weight: 400;

  &__link {
    color: #5a9f5e;
    text-decoration: none;
    transition: color 0.3s ease;

    &:hover {
      color: #4a8a4e;
    }
  }

  &__separator {
    color: #666666;
  }

  &__current {
    color: #000000;
    font-weight: 600;
  }
}

.product__wrapper {
  display: flex;
  gap: 40px;
  margin-bottom: 40px;
  @media screen and (max-width: 800px) {
    flex-direction: column;
    gap: 20px;
    align-items: center;
  }
}

.product__info-section {
  display: flex;
  flex-direction: column;
  gap: 30px;
  @media screen and (max-width: 900px) {
    gap: 20px;
  }
}

.product__title {
  color: #000000;
  font-family: 'Onest';
  font-size: 28px;
  font-weight: 700;
  line-height: 1.2;
  margin: 0;
  background: linear-gradient(135deg, #000000, #5a9f5e);
  background-clip: text;
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  @media screen and (max-width: 1200px) {
    font-size: 24px;
  }
  @media screen and (max-width: 900px) {
    font-size: 20px;
  }
  @media screen and (max-width: 635px) {
    font-size: 18px;
  }
}

.product__price {
  display: flex;
  align-items: center;
  gap: 20px;
}

.product__price-current {
  color: #000000;
  font-family: 'Onest';
  font-size: 28px;
  font-weight: 700;
  line-height: 1;
  @media screen and (max-width: 1200px) {
    font-size: 24px;
  }
  @media screen and (max-width: 900px) {
    font-size: 20px;
  }
  @media screen and (max-width: 635px) {
    font-size: 18px;
  }
}

.product__description {
  p {
    max-width: 600px;
    color: #666666;
    font-family: 'Onest';
    font-size: 16px;
    font-weight: 400;
    line-height: 1.6;
    margin: 0 0 20px 0;

    &:last-child {
      margin-bottom: 0;
    }
    @media screen and (max-width: 635px) {
      font-size: 14px;
    }
  }
}

.product__tabs {
  background: #ffffff;
  border-radius: 20px;
  box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
}

.product__tabs-header {
  display: flex;
  border-bottom: 1px solid #f0f0f0;
}

.product__tab-btn {
  flex: 1;
  background: transparent;
  border: none;
  padding: 20px 30px;
  font-family: 'Onest';
  font-size: 16px;
  font-weight: 600;
  color: #666666;
  cursor: pointer;
  transition: all 0.3s ease;
  position: relative;

  &:hover {
    color: #5a9f5e;
    background: #f8f9fa;
  }

  &--active {
    color: #5a9f5e;
    background: #f8f9fa;

    &::after {
      content: '';
      position: absolute;
      bottom: 0;
      left: 0;
      right: 0;
      height: 3px;
      background: #5a9f5e;
    }
  }
  @media screen and (max-width: 900px) {
    font-size: 14px;
    padding: 10px 10px;
  }
}

.product__tabs-content {
  padding: 40px 20px;
}

.product__tab-panel {
  animation: fadeIn 0.3s ease-in-out;
}

@keyframes fadeIn {
  from {
    opacity: 0;
    transform: translateY(10px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

.product__details-text {
  p {
    color: #666666;
    font-family: 'Onest';
    font-size: 16px;
    font-weight: 400;
    line-height: 1.6;
    margin: 0 0 20px 0;

    &:last-child {
      margin-bottom: 0;
    }
    @media screen and (max-width: 900px) {
      font-size: 14px;
    }
  }
}

.product__specifications-grid {
  display: flex;
  flex-direction: column;
  gap: 20px;
}

.product__spec-group {
  &-title {
    color: #000000;
    font-family: 'Onest';
    font-size: 18px;
    font-weight: 600;
    line-height: 1.2;
    margin: 0 0 20px 0;
    padding-bottom: 10px;
    border-bottom: 2px solid #5a9f5e;
    @media screen and (max-width: 900px) {
      font-size: 16px;
    }
  }
}

.product__spec-list {
  display: flex;
  flex-direction: column;
  gap: 12px;
  @media screen and (max-width: 900px) {
    gap: 16px;
  }
}

.product__spec-item {
  display: flex;
  justify-content: space-between;
  align-items: flex-start;
  gap: 20px;
  border-bottom: 1px solid #f0f0f0;

  &:last-child {
    border-bottom: none;
  }
  @media screen and (max-width: 900px) {
    flex-direction: column;
    gap: 5px;
  }
}

.product__spec-label {
  color: #666666;
  font-family: 'Onest';
  font-size: 14px;
  font-weight: 400;
  line-height: 1.4;
  flex: 1;
}

.product__spec-value {
  color: #000000;
  font-family: 'Onest';
  font-size: 14px;
  font-weight: 600;
  line-height: 1.4;
  text-align: right;
  flex: 1;
  @media screen and (max-width: 900px) {
    text-align: left;
  }
}
// :deep(.p-galleria-thumbnail) {
//   border-radius: 10px;
//   border: 1px solid #e5e7eb;
// }
:deep(.p-galleria-thumbnails-content) {
  display: none;
}
</style>
