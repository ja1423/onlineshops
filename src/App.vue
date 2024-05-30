<template>
  <div>
    <Header />
    <Products />
    <Intro />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Intro from "./components/Intro.vue";


export default {
  components: {
    Header,
    Intro,
    },
  data() {
    return {};
  },
};
</script>

<style lang="scss" scoped></style>


