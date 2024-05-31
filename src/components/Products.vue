<template>
  <div class="container">
    <div class="">
      <div class="text-3xl my-24">
        <h1>Успей купить</h1>
      </div>
      <div
        class="relative grid grid-cols-2 sm:grid-cols-1 md:grid-cols-6 gap-5"
      >
        <div v-for="(product, index) in data" :key="index">
          <Product :product="product" v-if="product.sale == true" />
        </div>

        <button
          class="gradient-border border border-gradien border-[#a446fc] py-2 flex flex-col items-center justify-end"
        >
          Все товары
        </button>
      </div>
    </div>
  </div>
</template>

<script setup>
import { reactive } from "vue";
import Product from "./SlideForProducts.vue";
const products = reactive([
  {
    img: "/images/boy 2.png",
    salePrice: 1999,
    sale: true,
    price: 2499,
    info: "Чехол для iphone 12 с дизайнерским принтом Super Shape 03",
  },
  {
    img: "/images/boy 1.png",
    salePrice: 3179,
    sale: true,
    price: 1999,
    info: "Футболка80 с дизайнерским принтом Super Shape 0201 абстракция на фиолетовом фоне",
  },
  {
    img: "/img/hat1.png",
    salePrice: 1999,
    sale: true,
    price: 1375,
    info: "Бейсболка с дизайнерским принтом Super Shape 01белая",
  },
  {
    img: "/img/phone1.png",
    salePrice: 599,
    sale: true,
    price: 1999,
    info: "Чехол для iphone 12 с дизайнерским принтом Super Shape 03",
  },

  {
    img: "/img/phone6.png",
    salePrice: 599,
    sale: true,
    price: 1999,
    info: "Чехол для iphone 12 с дизайнерским принтом Super Shape 03",
  },

  {
    img: "/img/boy2.png",
    salePrice: 2399,
    sale: true,
    price: 1999,
    info: "Футболка80 с дизайнерским принтом Super Shape 0201 абстракция на фиолетовом фоне",
  },

  {
    img: "/img/hat2.png",
    salePrice: 1375,
    sale: true,
    price: 1999,
    info: "Бейсболка с дизайнерским принтом Super Shape 01белая",
  },
  {
    img: "/img/phone9.png",
    salePrice: 599,
    sale: true,
    price: 2499,
    info: "Чехол для iphone 12 с дизайнерским принтом Super Shape 03",
  },

  {
    img: "/img/phone7.png",
    salePrice: 599,
    sale: true,
    price: 2499,
    info: "Чехол для iphone 12 с дизайнерским принтом Super Shape 03",
  },

  {
    img: "/img/boy3.png",
    salePrice: 1999,
    sale: true,
    price: 2499,
    info: "Футболка80 с дизайнерским принтом Super Shape 0201 абстракция на фиолетовом фоне",
  },
  {
    img: "/img/phone3.png",
    salePrice: 599,
    sale: true,
    price: 2499,
    info: "Чехол для iphone 12 с дизайнерским принтом Super Shape 03",
  },
  {
    img: "/img/boy5.png",
    salePrice: 2399,
    sale: true,
    price: 2499,
    info: "Футболка80 с дизайнерским принтом Super Shape 0201 абстракция на фиолетовом фоне",
  },
]);

const data = products.filter((item) => item.sale);
const data1 = products.filter((item) => !item.sale);
</script>

<style lang="scss" scoped></style>
