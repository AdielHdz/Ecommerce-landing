<template>
  <nav
    class="flex items-center border-b justify-between border-b-gray-200 py-8"
  >
    <div class="flex items-center">
      <a href="/" class="font-bold text-[30px] -translate-y-[2px] mr-[35px]"
        ><img src="../assets/images/logo.svg" alt=""
      /></a>
      <div class="flex items-center gap-4">
        <a
          href="#"
          class="text-md transition duration-200 text-gray-400 hover:text-black"
          >Collections</a
        >
        <a
          href="#"
          class="text-md transition duration-200 text-gray-400 hover:text-black"
          >Men</a
        >
        <a
          href="#"
          class="text-md transition duration-200 text-gray-400 hover:text-black"
          >Women</a
        >
        <a
          href="#"
          class="text-md transition duration-200 text-gray-400 hover:text-black"
          >About</a
        >
        <a
          href="#"
          class="text-md transition duration-200 text-gray-400 hover:text-black"
          >Contact</a
        >
      </div>
    </div>

    <div class="flex items-center gap-9">
      <img src="../assets/images/icon-cart.svg" alt="" />
      <img
        :src="avatar"
        alt=""
        class="rounded-full w-14 h-14 hover:cursor-pointer hover:border-[3px] hover:border-orange-400"
      />
    </div>
  </nav>
</template>

<script>
export default {
  name: "HeaderNav",
  props: ["avatar"],
};
</script>
