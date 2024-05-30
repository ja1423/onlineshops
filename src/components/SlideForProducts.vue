<script setup>
const props = defineProps({
  product: Object,
});
</script>
<template>
  <div class=" relative">
    <div
      class="group bg-white p-4 border rounded-md shadow-3xl w-full h-auto hover:absolute top-0 left-0 z-30 hover:scale-105 duration-200"
    >
      <div class="">
        <span
          v-if="product.sale == true"
          class="absolute text-[10px] border border-red-500 rounded-xl py-0.5 px-1 font-medium right-6 top-6"
          >-25%</span
        ><img class="w-full" :src="product.img" alt="" />
      </div>
      <div class="flex gap-2 items-center my-5">
        <p
          :class="product.sale ? 'text-[#FF4343]' : 'text-black'"
          class="text-[#FF4343] text-sm font-medium"
        >
          {{ product.salePrice }}₽
        </p>
        <div>
          <p
            v-if="product.sale == true"
            class="text-[#4646468C]/50 text-[10px] line-through decoration-red-500"
          >
            {{ product.price }}₽
          </p>
        </div>
      </div>
      <div class="group-hover:flex hidden">
        <p>4.9</p>
        <img class="px-1" src="/img/star.svg" alt="" />
        <p>14 отзывов</p>
      </div>
      <h3 class="text-sm uppercase my-2 hidden group-hover:block">Marple</h3>
      <p class="text-xs font-light">{{ product.info }}</p>
      <button
        class="group-hover:block hidden py-2 mt-3 bg-gradient-to-r from-purple-500 to-pink-500 text-white w-full"
      >
        В корзину
      </button>
    </div>
  </div>
</template>

<style lang="scss" scoped></style>