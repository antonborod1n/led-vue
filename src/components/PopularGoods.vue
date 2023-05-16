<template>
  <section class="popular">
    <div class="container">
      <h2 class="popular__title">Популярные товары —</h2>
      <div class="popular__inner">
        <div class="popular__item popular__tabs">
          <ul class="popular__tabs-list">
            <li
              class="popular__tabs-btn"
              v-for="(item, i) of popular"
              :key="i"
              @click="toggle"
            >
              {{ item.name }}
            </li>
          </ul>
        </div>
        <div class="popular__content">
          <div
            class="popular__content-item"
            v-for="(item, i) of popularItem"
            :key="i"
          >
            <img
              class="popular__content-img"
              :src="item.img"
              :alt="item.name"
            />
            <div class="popular__info-price">
              <h3 class="popular__subtitle">{{ item.name }}</h3>
              <div>
                <span class="popular__price">{{ item.price }}</span>
                <span class="popular__carrancy">{{ item.carrancy }}</span>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import { ref } from "vue";

const popular = [
  {
    name: "Одеяла",
  },
  {
    name: "Подушки",
  },
  {
    name: "Покрывала",
  },
  {
    name: "Пледы",
  },
  {
    name: "Простыни",
  },
  {
    name: "Наволочки",
  },
];

const popularItem = [
  {
    name: "Цокольный красный кирпич",
    img: "./src/assets/images/popular/1.png",
    price: "от 29",
    carrancy: "₽/шт",
  },
  {
    name: "Силикатный белый кирпич",
    img: "./src/assets/images/popular/2.png",
    price: "от 29",
    carrancy: "₽/шт",
  },
  {
    name: "Шамотный жаропрочный кирпич",
    img: "../src/assets/images/popular/3.png",
    price: "от 29",
    carrancy: "₽/шт",
  },
  {
    name: "Облицовочный фасадный кирпич",
    img: "./src/assets/images/popular/4.png",
    price: "от 29",
    carrancy: "₽/шт",
  },
  {
    name: "Печной кирпич",
    img: "./src/assets/images/popular/5.png",
    price: "от 29",
    carrancy: "₽/шт",
  },
];
</script>

