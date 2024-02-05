<template>
  <section class="pr-10 self-center">
    <h3 class="text-orange-400 font-semibold">SNEAKER COMPANY</h3>
    <h2 class="text-[40px] font-bold leading-10 mt-4">
      Fall Limited Edition Sneakers
    </h2>
    <p class="text-gray-500 mt-10">
      These low-profile sneakers are your perfect casual wear companion.
      Featuring a durable rubber outer sole, they´ll whistand everything the
      weather can offer.
    </p>

    <div class="flex items-center flex-wrap mt-5">
      <p class="text-[24px] font-bold mr-4">$125.00</p>
      <span
        class="inline-block bg-orange-100 px-2 rounded-sm font-semibold text-orange-600"
        >50%</span
      >
      <span class="block w-full font-semibold line-through text-gray-400"
        >$250.00</span
      >
    </div>
    <div class="flex gap-3 mt-6">
      <div
        class="bg-gray-100 flex gap-10 min-w-max px-4 font-bold h-[50px] rounded-xl items-center text-[18px]"
      >
        <img
          @click="
            () => {
              if (counter > 0) counter--;
            }
          "
          src="../assets/images/icon-minus.svg"
          alt=""
          class="cursor-pointer"
        />

        {{ counter }}

        <img
          @click="
            () => {
              counter++;
            }
          "
          src="../assets/images/icon-plus.svg"
          alt=""
          class="cursor-pointer"
        />
      </div>
      <button
        class="text-white bg-orange-300 w-full h-[50px] rounded-xl font-semibold flex items-center justify-center gap-2"
      >
        <img src="../assets/images/icon-cart-white.svg" alt="" />
        Add to cart
      </button>
    </div>
  </section>
</template>
<script>
import { ref } from "vue";

export default {
  name: "ProductInfo",
  setup() {
    const counter = ref(0);
    return { counter };
  },
};
</script>
