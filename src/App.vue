<template>
  <div class="container px-5 py-5">
    <div
      class="m-0 header"
      style="
        display: grid;
        grid-template-columns: 1fr 1fr 1fr;
        grid-gap: 20px;
        background: #48426d;
        border-radius: 20px;
        height: 80px;
        padding-top: 10px;
        box-shadow: 24px 24px 48px #353050, -24px -24px 48px #5b548a;
      "
    ></div>
    <header-app />
  </div>
</template>

<script>
import HeaderApp from "./components/HeaderApp.vue";
export default {
  components: {
    HeaderApp,
  },
};
</script>

<style>
.container {
  display: grid;
  grid-template-columns: 25% 75%;
  grid-gap: 30px;
}
</style>
