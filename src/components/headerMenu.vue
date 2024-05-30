<script>
export default {
  name: "menuHeader",
  data() {
    return {
      listMenu: [
        {
          gender: "Uomo",
          show: false,

          categories: [
            "T-shirt & Polo",
            "Felpe",
            "Jeans",
            "Pantaloni",
            "Giacche",
            "Tutto l'abbigliamento",
            "Camicie",
            "Pantaloni sportivi e Joggers",
            "Bermuda",
            "Moda mare",
            "Completi e cravatte",
          ],
        },
        {
          gender: "Donna",
          show: false,

          categories: [
            "T-shirt & Polo",
            "Felpe",
            "Jeans",
            "Pantaloni",
            "Giacche",
            "Tutto l'abbigliamento",
            "Camicie",
            "Pantaloni sportivi e Joggers",
            "Bermuda",
            "Moda mare",
            "Completi e cravatte",
          ],
        },
        {
          gender: "Bambini",
          show: false,
          categories: [
            "T-shirt & Polo",
            "Felpe",
            "Jeans",
            "Pantaloni",
            "Giacche",
            "Tutto l'abbigliamento",
            "Camicie",
            "Pantaloni sportivi e Joggers",
            "Bermuda",
            "Moda mare",
            "Completi e cravatte",
          ],
        },
      ],
    };
  },
};
</script>
<template>
  <div class="gender">
    <div class="genderContainer">
      <div class="dropDawnMenu" v-for="item in listMenu">
        <span @click="item.show = !item.show">{{ item.gender }}</span>
        <ul v-if="item.show">
          <li v-for="category in item.categories">{{ category }}</li>
        </ul>
      </div>
    </div>
  </div>
</template>
<style scoped>
.genderContainer {
  display: flex;
  color: white;
}
ul {
  top: 100%;
  list-style-type: none;
  position: absolute;
  background-color: gray;

  left: 0;
  right: 0;
  z-index: 2;
  display: flex;
  flex-wrap: wrap;
  padding: 10px;
}
li {
  margin: 10px 0;
  width: calc(100% / 5);
}
.dropDawnMenu {
  margin: 0 10px;
}
</style>
