<template>
    <div class="container">
        <div class="flex">
            <div class="text-3xl mx-72 my-24">
                <h1>Успей купить</h1>
            </div>
            <div
          class="relative grid grid-cols-2 sm:grid-cols-1 md:grid-cols-6 gap-5"
        >
          <div v-for="(product, index) in products" :key="index">
            <Product :product="product" v-if="product.sale == true" />
          </div>
          <button
            class="gradient-border border border-gradien py-2 flex flex-col items-center justify-end"
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
    img: "/images/boy 1.png",
    salePrice: 1999,
    sale: true,
    price: 2499,
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
    img: "/images/boy 1.png",
    salePrice: 1999,
    sale: true,
    price: 2499,
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
    img: "/img/phone1.png",
    salePrice: 1999,
    sale: false,
    price: 2499,
    info: "Чехол для iphone 12 с дизайнерским принтом Super Shape 03",
  },
  {
    img: "/img/phone2.png",
    salePrice: 1999,
    sale: false,
    price: 2499,
    info: "Чехол для iphone 12 с дизайнерским принтом Super Shape 03",
  },
  {
    img: "/img/boy1.png",
    salePrice: 1999,
    sale: true,
    price: 2499,
    info: "Чехол для iphone 12 с дизайнерским принтом Super Shape 03",
  },
  {
    img: "/img/boy2.png",
    salePrice: 1999,
    sale: false,
    price: 2499,
    info: "Чехол для iphone 12 с дизайнерским принтом Super Shape 03",
  },
  {
    img: "/img/hat3.png",
    salePrice: 1999,
    sale: true,
    price: 2499,
    info: "Чехол для iphone 12 с дизайнерским принтом Super Shape 03",
  },
  {
    img: "/img/phone1.png",
    salePrice: 1999,
    sale: false,
    price: 2499,
    info: "Чехол для iphone 12 с дизайнерским принтом Super Shape 03",
  },
  {
    img: "/img/phone2.png",
    salePrice: 1999,
    sale: true,
    price: 2499,
    info: "Чехол для iphone 12 с дизайнерским принтом Super Shape 03",
  },
  {
    img: "/img/hat3.png",
    salePrice: 1999,
    sale: true,
    price: 2499,
    info: "Чехол для iphone 12 с дизайнерским принтом Super Shape 03",
  },
  {
    img: "/img/phone1.png",
    salePrice: 1999,
    sale: false,
    price: 2499,
    info: "Чехол для iphone 12 с дизайнерским принтом Super Shape 03",
  },
  {
    img: "/img/phone2.png",
    salePrice: 1999,
    sale: false,
    price: 2499,
    info: "Чехол для iphone 12 с дизайнерским принтом Super Shape 03",
  },
  {
    img: "/img/phone1.png",
    salePrice: 1999,
    sale: false,
    price: 2499,
    info: "Чехол для iphone 12 с дизайнерским принтом Super Shape 03",
  },
  {
    img: "/img/phone2.png",
    salePrice: 1999,
    sale: false,
    price: 2499,
    info: "Чехол для iphone 12 с дизайнерским принтом Super Shape 03",
  },
  {
    img: "/img/boy1.png",
    salePrice: 1999,
    sale: true,
    price: 2499,
    info: "Чехол для iphone 12 с дизайнерским принтом Super Shape 03",
  },
  {
    img: "/img/boy2.png",
    salePrice: 1999,
    sale: false,
    price: 2499,
    info: "Чехол для iphone 12 с дизайнерским принтом Super Shape 03",
  },
  {
    img: "/img/boy1.png",
    salePrice: 1999,
    sale: true,
    price: 2499,
    info: "Чехол для iphone 12 с дизайнерским принтом Super Shape 03",
  },
  {
    img: "/img/boy2.png",
    salePrice: 1999,
    sale: true,
    price: 2499,
    info: "Чехол для iphone 12 с дизайнерским принтом Super Shape 03",
  },
  {
    img: "/img/phone1.png",
    salePrice: 1999,
    sale: false,
    price: 2499,
    info: "Чехол для iphone 12 с дизайнерским принтом Super Shape 03",
  },
  {
    img: "/img/phone2.png",
    salePrice: 1999,
    sale: false,
    price: 2499,
    info: "Чехол для iphone 12 с дизайнерским принтом Super Shape 03",
  },
  {
    img: "/img/boy1.png",
    salePrice: 1999,
    sale: true,
    price: 2499,
    info: "Чехол для iphone 12 с дизайнерским принтом Super Shape 03",
  },
  {
    img: "/img/boy2.png",
    salePrice: 1999,
    sale: false,
    price: 2499,
    info: "Чехол для iphone 12 с дизайнерским принтом Super Shape 03",
  },
  {
    img: "/img/hat3.png",
    salePrice: 1999,
    sale: true,
    price: 2499,
    info: "Чехол для iphone 12 с дизайнерским принтом Super Shape 03",
  },
  {
    img: "/img/phone1.png",
    salePrice: 1999,
    sale: false,
    price: 2499,
    info: "Чехол для iphone 12 с дизайнерским принтом Super Shape 03",
  },
  {
    img: "/img/phone2.png",
    salePrice: 1999,
    sale: true,
    price: 2499,
    info: "Чехол для iphone 12 с дизайнерским принтом Super Shape 03",
  },
  {
    img: "/img/hat3.png",
    salePrice: 1999,
    sale: true,
    price: 2499,
    info: "Чехол для iphone 12 с дизайнерским принтом Super Shape 03",
  },
  {
    img: "/img/phone1.png",
    salePrice: 1999,
    sale: false,
    price: 2499,
    info: "Чехол для iphone 12 с дизайнерским принтом Super Shape 03",
  },
  {
    img: "/img/phone2.png",
    salePrice: 1999,
    sale: false,
    price: 2499,
    info: "Чехол для iphone 12 с дизайнерским принтом Super Shape 03",
  },
  {
    img: "/img/hat3.png",
    salePrice: 1999,
    sale: true,
    price: 2499,
    info: "Чехол для iphone 12 с дизайнерским принтом Super Shape 03",
  },
  {
    img: "/img/phone1.png",
    salePrice: 1999,
    sale: false,
    price: 2499,
    info: "Чехол для iphone 12 с дизайнерским принтом Super Shape 03",
  },
  {
    img: "/img/phone2.png",
    salePrice: 1999,
    sale: true,
    price: 2499,
    info: "Чехол для iphone 12 с дизайнерским принтом Super Shape 03",
  },
  {
    img: "/img/hat3.png",
    salePrice: 1999,
    sale: true,
    price: 2499,
    info: "Чехол для iphone 12 с дизайнерским принтом Super Shape 03",
  },
  {
    img: "/img/phone1.png",
    salePrice: 1999,
    sale: false,
    price: 2499,
    info: "Чехол для iphone 12 с дизайнерским принтом Super Shape 03",
  },
  {
    img: "/img/phone2.png",
    salePrice: 1999,
    sale: false,
    price: 2499,
    info: "Чехол для iphone 12 с дизайнерским принтом Super Shape 03",
  },
]);
</script>

<style lang="scss" scoped>

</style>