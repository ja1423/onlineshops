<template>
    <div class="container">
        <div class="">
            <div class="text-3xl my-24">
                <h1>Магазины для вас</h1>
            </div>
             <div
        class="relative grid grid-cols-2 sm:grid-cols-1 md:grid-cols-4 gap-5"
      >
        <div v-for="(product, index) in data" :key="index">
          <Product :product="product" v-if="product.sale == true" />
        </div>
      </div>
        </div>

    </div>
</template>

<script>
export default {
    setup () {
        

        return {}
    }
}
</script>

<style lang="scss" scoped>

</style>