<template>
  <section class="grid pl-10 gap-5">
    <img
      v-if="imgElement === 1"
      src="../assets/images/image-product-1.jpg"
      alt=""
      class="w-full rounded-md"
    />
    <img
      v-if="imgElement === 2"
      src="../assets/images/image-product-2.jpg"
      alt=""
      class="w-full rounded-md"
    />
    <img
      v-if="imgElement === 3"
      src="../assets/images/image-product-3.jpg"
      alt=""
      class="w-full rounded-md"
    />
    <img
      v-if="imgElement === 4"
      src="../assets/images/image-product-4.jpg"
      alt=""
      class="w-full rounded-md"
    />
    <div class="grid grid-cols-4 gap-5">
      <img
        src="../assets/images/image-product-1.jpg"
        alt=""
        @click="imgElement = 1"
        :class="[
          'rounded-md cursor-pointer hover:border-orange-400 hover:opacity-50',
          {
            'border-[3px] border-orange-400 opacity-50': imgElement === 1,
          },
        ]"
      />
      <img
        src="../assets/images/image-product-2.jpg"
        alt=""
        @click="imgElement = 2"
        :class="[
          'rounded-md cursor-pointer  hover:border-orange-400 hover:opacity-50',
          {
            'border-[3px] border-orange-400 opacity-50': imgElement === 2,
          },
        ]"
      />

      <img
        src="../assets/images/image-product-3.jpg"
        alt=""
        @click="imgElement = 3"
        :class="[
          'rounded-md cursor-pointer  hover:border-orange-400 hover:opacity-50',
          {
            'border-[3px] border-orange-400 opacity-50': imgElement === 3,
          },
        ]"
      />

      <img
        src="../assets/images/image-product-4.jpg"
        alt=""
        @click="imgElement = 4"
        :class="[
          'rounded-md cursor-pointer  hover:border-orange-400 hover:opacity-50',
          {
            'border-[3px] border-orange-400 opacity-50': imgElement === 4,
          },
        ]"
      />
    </div>
  </section>
</template>
<script>
import { ref } from "vue";

export default {
  name: "Carousel",
  setup() {
    const imgElement = ref(1);

    return { imgElement };
  },
};
</script>
