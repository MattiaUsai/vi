<script>
import headerMenu from "./headerMenu.vue";
export default {
  name: "headerComponent",
  components: {
    headerMenu,
  },
};
</script>
<template>
  <header>
    <!-- imposta la larghezza a 25%  categorie uomo donna bambino-->
    <div class="col-25">
      <headerMenu />
    </div>
    <!-- larghezza 50% logo al centro della pagina -->
    <div class="col-50 h-logo">
      <img class="logo" src="/img/boolean-logo.png" alt="" />
    </div>
    <!-- bottoni carello, accedi e preferiti -->
    <div class="col-25 buttons">
      <button class="prefered">&hearts;</button>
      <button class="shop"></button>
      <button class="button">&#128100;</button>
    </div>
  </header>
</template>
<style scoped>
button {
  background: orange;
  border: none;
  color: white;
}
header {
  position: relative;
  display: flex;
  align-items: center;
}
.h-logo img {
  width: 50%;
}
.buttons {
  text-align: right;
}
</style>
