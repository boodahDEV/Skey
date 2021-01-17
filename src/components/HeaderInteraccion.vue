<template>
  <div class="m-0 contenedor">
    <button class="btn button-option">Seleccionar</button>
    <button class="btn button-option" style="width: 80px">Editar</button>
    <button class="btn button-option" style="width: 80px">Eliminar</button>
  </div>
</template>

<script>
export default {
  name: "HeaderInteraccion",
};
</script>

<style scoped>
.contenedor {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  grid-gap: 8px;
  background: #48426d;
  border-radius: 30px;
  height: 50px;
  padding-top: 10px;
  box-shadow: 4px 4px 15px 0px rgba(0, 0, 0, 0.66);
}

.button-option {
  width: 120px;
  height: 30px;
  margin-left: 8px;
  margin-right: 8px;
  padding: 3px;
  border-radius: 100px;
  cursor: pointer;
  border: none;
  outline: none;
  backdrop-filter: blur(20px);
  align-items: center;
  justify-content: center;
  color: #fff;
  font-weight: bold;
  overflow: hidden;
  font-family: "Roboto Mono", monospace;

  font-size: 15px;
  font-weight: 800;
}

.button-option:hover::before {
  top: 0px;
  border-radius: 0;
}

.button-option::before {
  content: "";
  position: absolute;
  top: 30px;
  left: 0px;
  width: 100%;
  height: 100%;
  background-color: #f0c38e;
  border-radius: 95%;
  z-index: -1;
  transition: all 0.3s;
}
</style>