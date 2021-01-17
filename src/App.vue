<template>
  <div class="container px-5 py-5">
    <div
      class="m-0"
      style="
        display: grid;
        grid-template-columns: 1fr 1fr 1fr;
        grid-gap: 20px;
        background: #48426d;
        border-radius: 20px;
        height: 82px;
        padding-top: 10px;
        box-shadow: 24px 24px 48px #353050, -24px -24px 48px #5b548a;
        grid-column: 1 / 2;
        grid-row: 1 / 3;
      "
    >
     
    </div>
    <header-app />
    <contenedor-grupo-app/>
    
  </div>
</template>

<script>
import ContenedorGrupoApp from './components/ContenedorGrupoApp.vue';
import HeaderApp from "./components/HeaderApp.vue";
export default {
  components: {
    HeaderApp,
    ContenedorGrupoApp,
  },
};
</script>

<style scoped>
.container {
  display: grid;
  grid-template-columns: 25% 75%;
  grid-template-rows: 1fr 7fr;
  grid-column-gap: 30px;
  grid-row-gap: 50px;
}
</style>
