<template>
  <div>
    <HomeCatalog />
    <HomeService />
    <HomeReviews />
    <HomeAbout />
  </div>
</template>

<script lang="ts" setup>
useHead({
  title: 'ZENIT - Лазерные уровни, шуруповерты, угловые шлифовальные машины',
  meta: [
    {
      name: 'description',
      content:
        'Продажа и обслуживание лазерных уровней, шуруповертов, угловых шлифовальных машин',
    },
    {
      property: 'og:title',
      content:
        'ZENIT - Лазерные уровни, шуруповерты, угловые шлифовальные машины',
    },
    {
      property: 'og:description',
      content:
        'Продажа и обслуживание лазерных уровней, шуруповертов, угловых шлифовальных машин',
    },
    { property: 'og:type', content: 'website' },
    { property: 'og:url', content: 'https://zenit-tools.ru/' },
    { property: 'og:site_name', content: 'ZENIT' },
    { property: 'og:locale', content: 'ru_RU' },
    { name: 'robots', content: 'index, follow' },
  ],
})
</script>

<style></style>
