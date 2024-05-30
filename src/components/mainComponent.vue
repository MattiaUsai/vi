<script>
export default {
  name: "mainComponent",
};
</script>
<template>
  <main>
    <!-- struttura layaut 1 riga 3 colonne  -->
    <div class="row">
      <!-- larghezza massima 1200px -->
      <div class="container">
        <!-- imposta la larghezza del contenuto a 1/3 della larghezza del container  -->

        <div class="content col-33">
          <!-- immagine prodotto -->
          <img class="view" src="/img/1.webp" alt="" />
          <!-- immagine da visualizzare al passare del mouse -->
          <img class="hover" src="/img/1b.webp" alt="" />
          <!-- contenitore cuori per aggiungere ai preferiti  -->
          <div class="heart-contain">
            <!-- cuore diventa rosso al passare del mouse -->
            <span class="heart-view">&hearts;</span>
            <span class="heart-hover">&hearts;</span>
          </div>
          <!-- marca prodotto -->
          <span class="mark">levi&#8217;s</span>
          <!-- nome del prodotto  -->
          <h2 class="name">relaxed fit tee unisex</h2>
          <!-- prezzo del prodotto  -->
          <span class="price">14,99&euro;</span>
          <!-- vecchio prezzo del prodotto  -->
          <span class="ex-price">29,00&euro;</span>
          <div class="info-img">
            <!-- sconto  -->
            <span class="bg-red info">50&percnt;</span>
            <!-- sostenibilita -->
            <span class="bg-green info">sostenibile</span>
          </div>
        </div>

        <div class="content col-33">
          <img class="view" src="/img/2.webp" alt="" />
          <img class="hover" src="/img/2b.webp" alt="" />
          <div class="heart-contain">
            <span class="heart-view">&hearts;</span>
            <span class="heart-hover">&hearts;</span>
          </div>
          <span class="mark">guess</span>
          <h2 class="name">roses tee</h2>
          <span class="price">20,99&euro;</span>
          <span class="ex-price">29,00&euro;</span>
          <div class="info-img">
            <span class="bg-red info">50&percnt;</span>
          </div>
        </div>

        <div class="content col-33">
          <img class="view" src="/img/3.webp" alt="" />
          <img class="hover" src="/img/3b.webp" alt="" />
          <div class="heart-contain">
            <span class="heart-view">&hearts;</span>
            <span class="heart-hover">&hearts;</span>
          </div>
          <span class="mark">come zucchero filato</span>
          <h2 class="name">voglia di colori pastello</h2>
          <span class="price">129,99&euro;</span>
          <span class="ex-price">184,00&euro;</span>
          <div class="info-img">
            <span class="bg-red info">50&percnt;</span>
          </div>
        </div>

        <div class="content col-33">
          <img class="view" src="/img/4.webp" alt="" />
          <img class="hover" src="/img/4b.webp" alt="" />
          <div class="heart-contain">
            <span class="heart-view">&hearts;</span>
            <span class="heart-hover">&hearts;</span>
          </div>
          <span class="mark">levi&#8217;s</span>
          <h2 class="name">tee unisex</h2>
          <span class="price">14,99&euro;</span>
          <span class="ex-price">29,00&euro;</span>
          <div class="info-img">
            <span class="bg-red info">50&percnt;</span>
            <span class="bg-green info">sostenibile</span>
          </div>
        </div>

        <div class="content col-33">
          <img class="view" src="/img/5.webp" alt="" />
          <img class="hover" src="/img/5b.webp" alt="" />
          <div class="heart-contain">
            <span class="heart-view">&hearts;</span>
            <span class="heart-hover">&hearts;</span>
          </div>
          <span class="mark">maya deluxe</span>
          <h2 class="name">stripe bodice</h2>
          <span class="price">99,99&euro;</span>
        </div>

        <div class="content col-33">
          <img class="view" src="/img/6.webp" alt="" />
          <img class="hover" src="/img/6b.webp" alt="" />
          <div class="heart-contain">
            <span class="heart-view">&hearts;</span>
            <span class="heart-hover">&hearts;</span>
          </div>
          <span class="mark">esprit</span>
          <h2 class="name">maglione-blackx</h2>
          <span class="price">29,99&euro;</span>
          <div class="info-img">
            <span class="bg-green info">sostenibile</span>
          </div>
        </div>
      </div>
    </div>
  </main>
</template>
<style></style>
