<template>
  <div class="container mx-auto mt-5 px-3">
    <div>
      <div class="text-3xl my-24 text-center md:text-left">
        <h1>Рекомендуемые для вас товар</h1>
      </div>
      <div class="relative grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 lg:grid-cols-6 gap-5 shadow-lg">
        <div v-for="(product, index) in data" :key="index">
          <Product :product="product" v-if="product.sale" />
        </div>
      </div>
      <div class="flex justify-center md:justify-end w-full my-4">
        <button class="gradient-border border border-gradien border-[#a446fc] py-2 px-4">
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
    img: "/img/phone3.png",
    salePrice: 599,
    sale: true,
    price: 2499,
    info: "Чехол для iphone 12 с дизайнерским принтом Super Shape 03",
  },
  {
    img: "/img/boy4.png",
    salePrice: 1999,
    sale: true,
    info: "Футболка с дизайнерским принтом Super Shape 04 формулы",
  },
  {
    img: "/img/phone4.png",
    salePrice: 1999,
    sale: true,
    info: "Чехол для iphone 12 с дизайнерским принтом Super Shape 03",
  },
  {
    img: "/img/phone5.png",
    salePrice: 1999,
    sale: true,
    info: "Чехол для iphone 12 с дизайнерским принтом Super Shape 03",
  },
  {
    img: "/images/boy 2.png",
    salePrice: 1999,
    sale: true,
    price: 2499,
    info: "Чехол для iphone 12 с дизайнерским принтом Super Shape 03",
  },
  {
    img: "/img/hat3.png",
    salePrice: 599,
    sale: true,
    info: "Бейсболка с дизайнерским принтом Super Shape 01белая",
  },
  {
    img: "/images/boy 2.png",
    salePrice: 1999,
    sale: true,
    price: 2499,
    info: "Чехол для iphone 12 с дизайнерским принтом Super Shape 03",
  },
  {
    img: "/images/t-shirt9 1.png",
    salePrice: 1375,
    sale: true,
    info: "Футболка с дизайнерским принтом Super Shape 04 формулы",
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
  {
    img: "/img/phone5.png",
    salePrice: 1999,
    sale: true,
    info: "Чехол для iphone 12 с дизайнерским принтом Super Shape 03",
  },
  {
    img: "/img/phone8.png",
    salePrice: 1999,
    sale: true,
    info: "Чехол для iphone 12 с дизайнерским принтом Super Shape 03",
  },
  {
    img: "/img/phone9.png",
    salePrice: 1999,
    sale: true,
    info: "Чехол для iphone 12 с дизайнерским принтом Super Shape 03",
  },
  {
    img: "/img/phone8.png",
    salePrice: 1999,
    sale: true,
    info: "Чехол для iphone 12 с дизайнерским принтом Super Shape 03",
  },
  {
    img: "/img/boy4.png",
    salePrice: 1999,
    sale: true,
    info: "Футболка с дизайнерским принтом Super Shape 04 формулы",
  },
  {
    img: "/img/t-shirt5.png",
    salePrice: 2399,
    sale: true,
    info: "Футболка с дизайнерским принтом Super Shape 04 формулы",
  },
  {
    img: "/images/boy 2.png",
    salePrice: 1999,
    sale: true,
    price: 2499,
    info: "Чехол для iphone 12 с дизайнерским принтом Super Shape 03",
  },
  {
    img: "/img/phone4.png",
    salePrice: 1999,
    sale: true,
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
    img: "/img/boy3.png",
    salePrice: 1999,
    sale: true,
    price: 2499,
    info: "Футболка80 с дизайнерским принтом Super Shape 0201 абстракция на фиолетовом фоне",
  },

  {
    img: "/img/phone1.png",
    salePrice: 599,
    sale: true,
    price: 1999,
    info: "Чехол для iphone 12 с дизайнерским принтом Super Shape 03",
  },
   {
    img: "/images/t-shirt9 1.png",
    salePrice: 1375,
    sale: true,
    info: "Футболка с дизайнерским принтом Super Shape 04 формулы",
  },
    {
    img: "/img/phone9.png",
    salePrice: 599,
    sale: true,
    price: 2499,
    info: "Чехол для iphone 12 с дизайнерским принтом Super Shape 03",
  },
  {
    img: "/img/t-shirt2.png",
    salePrice: 2399,
    sale: true,
    info: "Футболка с дизайнерским принтом Super Shape 04 формулы",
  },

  {
    img: "/img/phone9.png",
    salePrice: 1999,
    sale: true,
    info: "Чехол для iphone 12 с дизайнерским принтом Super Shape 03",
  },
  {
    img: "/img/phone8.png",
    salePrice: 1999,
    sale: true,
    info: "Чехол для iphone 12 с дизайнерским принтом Super Shape 03",
  },
  {
    img: "/img/boy4.png",
    salePrice: 1999,
    sale: true,
    info: "Футболка с дизайнерским принтом Super Shape 04 формулы",
  },
   {
    img: "/img/t-shirt5.png",
    salePrice: 2399,
    sale: true,
    info: "Футболка с дизайнерским принтом Super Shape 04 формулы",
  },

 
]);

const data = products.filter((item) => item.sale);
const data1 = products.filter((item) => !item.sale);
</script>

<style lang="scss" scoped></style>
