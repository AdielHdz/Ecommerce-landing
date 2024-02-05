<template>
  <section class="py-[60px] px-[30px] gap-20 grid grid-cols-2">
    <Carousel />
    <ProductInfo />
  </section>
</template>

<script>
import { onMounted, ref } from "vue";
import Carousel from "./Carousel.vue";
import ProductInfo from "./ProductInfo.vue";
export default {
  name: "PanelProduct",
  components: {
    Carousel,
    ProductInfo,
  },
};
</script>
