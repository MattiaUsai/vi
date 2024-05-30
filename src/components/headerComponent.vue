<script>
export default {
  name: "headerComponent",
};
</script>
<template>
  <header>
    <div class="container">
      <!-- imposta la larghezza a 25%  categorie uomo donna bambino-->
      <div class="col-25">
        <div class="categories">
          <button class="category">Uomo</button>
          <button class="category">Donna</button>
          <button class="category">Bambino</button>
        </div>
      </div>
      <!-- larghezza 50% logo al centro della pagina -->
      <div class="col-50 h-logo">
        <img class="logo" src="/img/boolean-logo.png" alt="" />
      </div>
      <!-- bottoni carello, accedi e preferiti -->
      <div class="col-25 buttons">
        <button class="button">&hearts;</button>
        <button class="button shop">
          <img class="shopp" src="/img/carrello.png" alt="" />
        </button>
        <button class="button">&#128100;</button>
      </div>
    </div>
  </header>
</template>
<style scoped>
button {
  background: orange;
  border: none;
  color: white;
}
</style>
