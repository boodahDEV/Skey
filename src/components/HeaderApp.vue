/* eslint-disable no-mixed-spaces-and-tabs */
<template>
  <div class="card header">
    <div class="card-body header-content">
      <button class="btn button" style="color: #fff">Crear</button>
      <header-interaccion />
    </div>
  </div>
</template>

<script>
import HeaderInteraccion from "./HeaderInteraccion.vue";
export default {
  components: { HeaderInteraccion },
  name: "HeaderApp",
};
</script>

<style scoped>
.header {
  background-color: #f0c38e;
  border-radius: 20px;
  border: 0px;
  border-color: #fff;
  box-shadow: 24px 24px 48px #353050, -24px -24px 48px #5b548a;
  /* padding-top: 10px; */
}

.header-content {
  display: grid;
  grid-gap: 5px;
  grid-template-columns: 1fr 1fr 1fr;
  height: 82px;
}

.button {
  width: 150px;
  height: 50px;
  padding: 10px;
  border-radius: 100px;
  background-color: #48426d;
  cursor: pointer;
  border: none;
  outline: none;
  backdrop-filter: blur(20px);
  align-items: center;
  justify-content: center;
  color: #fff;
  overflow: hidden;
  font-family: 'Roboto Mono', monospace;
  font-size: 15px;
  box-shadow: 4px 4px 15px 0px rgba(0, 0, 0, 0.66);
  /* text-transform: uppercase; */
  font-weight: 800;
}
.button:hover::before {
  top: 0px;
  border-radius: 0;
}

.button::before {
  content: "";
  position: absolute;
  top: 60px;
  left: 0px;
  width: 100%;
  height: 100%;
  background-color: #312051;
  border-radius: 95%;
  z-index: -1;
  transition: all 0.3s;
}
</style>