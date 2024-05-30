<script>
export default {
  name: "mainComponent",
  data() {
    return {
      productlist: [
        {
          name: "relaxed fit tee unisex",
          brand: "Levi&#8217;s",
          price: "14,99&euro;",
          exPrice: "29,00&euro;",
          img: "/img/1.webp",
          imgHover: "/img/1b.webp",
          show: true,
          color: "white",
          discount: "50%",
          eGreen: true,
        },
        {
          name: "roses tee",
          brand: "Guess",
          price: "20,99&euro;",
          exPrice: "29,00&euro;",
          img: "/img/2.webp",
          imgHover: "/img/2b.webp",
          show: true,
          color: "white",
          discount: "50%",
          eGreen: false,
        },
        {
          name: "voglia di colori pastello",
          brand: "come zucchero filato",
          price: "129,99&euro;",
          exPrice: "184,00&euro;",
          img: "/img/3.webp",
          imgHover: "/img/3b.webp",
          show: true,
          color: "white",
          discount: "50%",
          eGreen: false,
        },
        {
          name: "tee unisex",
          brand: "Levi&#8217;s",
          price: "14,99&euro;",
          exPrice: "29,00&euro;",
          img: "/img/4.webp",
          imgHover: "/img/4b.webp",
          show: true,
          color: "white",
          discount: "50%",
          eGreen: true,
        },
        {
          name: "stripe bodice",
          brand: "Maya deluxe",
          price: "99,99&euro;",
          exPrice: "",
          img: "/img/5.webp",
          imgHover: "/img/5b.webp",
          show: true,
          color: "white",
          discount: "",
          eGreen: false,
        },
        {
          name: "maglione black",
          brand: "esprit",
          price: "29,99&euro;",
          exPrice: "",
          img: "/img/6.webp",
          imgHover: "/img/6b.webp",
          show: true,
          color: "white",
          discount: "",
          eGreen: true,
        },
      ],
    };
  },
};
</script>
<template>
  <main>
    <!-- struttura layaut 1 riga 3 colonne  -->
    <div class="row">
      <!-- larghezza massima 1200px -->
      <div class="container">
        <!-- imposta la larghezza del contenuto a 1/3 della larghezza del container  -->

        <div class="content col-33" v-for="product in productlist">
          <!-- immagine prodotto -->
          <img class="view" :src="product.img" alt="" />
          <!-- immagine da visualizzare al passare del mouse -->
          <img class="hover" :src="product.imgHover" alt="" />
          <!-- contenitore cuori per aggiungere ai preferiti  -->
          <div class="heart-contain">
            <!-- cuore diventa rosso al passare del mouse -->
            <span class="heart-view">&hearts;</span>
            <span class="heart-hover">&hearts;</span>
          </div>
          <!-- marca prodotto -->
          <span class="mark">{{ product.brand }}</span>
          <!-- nome del prodotto  -->
          <h2 class="name">{{ product.name }}</h2>
          <!-- prezzo del prodotto  -->
          <span class="price">{{ product.price }}</span>
          <!-- vecchio prezzo del prodotto  -->
          <span class="ex-price">{{ product.exPrice }}</span>
          <div class="info-img">
            <!-- sconto  -->
            <span class="bg-red info" v-if="product.discount">{{
              product.discount
            }}</span>
            <!-- sostenibilita -->
            <span class="bg-green info" v-show="product.eGreen"
              >sostenibile</span
            >
          </div>
        </div>
      </div>
    </div>
  </main>
</template>
<style></style>
