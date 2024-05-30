<template>
  <div>
    <Header />
    <Intro />
    <Products />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Products from "./components/Products.vue";
import Intro from "./components/Intro.vue";


export default {
  components: {
    Header,
    Intro,
    Products,
    },
  data() {
    return {};
  },
};
</script>

<style lang="scss" scoped></style>


