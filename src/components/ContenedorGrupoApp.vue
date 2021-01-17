<template>
  <div class="grupo-area">

  </div>
</template>

<script>
export default {
    name:"ContenedorGrupoApp"
}
</script>

<style scoped>
    .grupo-area{
        display: grid;
        grid-template-columns: 1fr 1fr 1fr 1fr;
        grid-gap: 10px;
        height: 500px;
        background-color: #48426d;
        border-radius: 20px;
                box-shadow: 24px 24px 98px #353050, -24px -24px 48px #5b548a;

    }

</style>