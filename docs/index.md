---
layout: home
editLink: false
footer: true

hero:
  name: Vue Yandex Maps
  text: Обертка для<br>Яндекс Карт 3.0
  tagline: Легковесная, упакована с поддержкой<br>SSR и TypeScript из коробки.
  actions:
    - theme: brand
      text: Начало работы
      link: /guide/about
    - theme: alt
      text: Переход с 0.x/1.x
      link: /guide/migration
    - theme: alt
      text: Открыть на Github
      link: https://github.com/PNKBizz/vue-yandex-maps

features:
  - icon: 🚀
    title: Легковесная
    details: "Всего одна зависимость: типы Яндекс Карт.<br><br>Библиотека весит всего ~150Кб с учётом всех типов и без минификации."
  - icon: ⚙️
    title: Настраиваемая
    details: Все компоненты передают оригинальный инстанс Яндекса в v-model.<br><br>А обновлять версию @yandex/ymaps3-types и использовать новые возможности можно силами разработчика!
  - icon: 🦾
    title: Современная
    details: Библиотека использует ES Modules, поддерживает Tree Shaking и написана на TypeScript.<br><br>Кроме того, она поставляется без полифиллов!
  - icon: ⭐
    title: Доступная
    details: Поддержаны Vue 3 и Nuxt 3 - на Webpack и Vite. Реализована, пусть с особенностями, даже поддержка Vue 2 с Nuxt 2!<br><br>Библиотека поставляется с полным набором компонентов Карт 3.0.
---

<style>
:root {
  --vp-home-hero-name-color: #FF5B4D;
}
</style>
