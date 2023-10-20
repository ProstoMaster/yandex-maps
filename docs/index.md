---
layout: home
editLink: false
footer: true

hero:
  name: Vue Yandex Maps
  text: Обертка для<br>Яндекс Карт 3.0.
  tagline: Легковесная, упакована с поддержкой<br>SSR и TypeScript из коробки.
  actions:
    - theme: brand
      text: Начало работы
      link: /guide/about
    - theme: alt
      text: Открыть на Github
      link: https://github.com/PNKBizz/vue-yandex-maps/tree/v2

features:
  - icon: 🚀
    title: Легковесная
    details: "У нас всего две зависимости: типы Карт и @nuxt/kit для поддержки Nuxt.<br><br>Проект написан на ES Modules и регистрирует только те компоненты, что вы используете (Tree Shaking).<br><br>Библиотека со всеми типами и файлами весит всего 187Кб, а вес основного файла после минификации - 24Кб."
  - icon: 🛠️
    title: Широкая кастомизация
    details: Требуется доступ к Картам?<br>Не беда - все компоненты передают свои инстансы в v-model наверх для удобства разработчика<br><br>Яндекс выпустили апдейт? Обновите версию @yandex/ymaps3-types и используйте новые возможности, не дожидаясь авторов библиотеки.
  - icon: ⭐
    title: Поддержано всё, и больше
    details: Поддержаны Vue 3 и Nuxt 3 - на Webpack и Vite. Реализована, пусть с особенностями, даже поддержка Vue 2 с Nuxt 2!<br><br>Библиотека поставляется с полным набором компонентов Карт 3.0 и написана на TypeScript.
---

<style>
:root {
  --vp-home-hero-name-color: #FF5B4D;
}
</style>
