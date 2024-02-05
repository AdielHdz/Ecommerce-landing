<template>
  <section class="max-w-[1280px] m-auto">
    <HeaderNav :avatar="avatar" />
    <PanelProduct />
  </section>
</template>
<script>
import { onMounted, ref } from "vue";
import HeaderNav from "./HeaderNav.vue";
import PanelProduct from "./PanelProduct.vue";
export default {
  name: "HelloWorld",
  components: { HeaderNav, PanelProduct },
  setup() {
    const avatar = ref();

    onMounted(() => {
      fetch("https://reqres.in/api/users/6")
        .then((response) => response.json())
        .then((data) => (avatar.value = data.data.avatar));
    });

    return {
      avatar,
    };
  },
};
</script>
