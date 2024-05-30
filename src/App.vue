<script>
import headerComponent from "./components/headerComponent.vue";
import footerComponent from "./components/footerComponent.vue";
import mainComponent from "./components/mainComponent.vue";

export default {
  components: {
    headerComponent,
    mainComponent,
    footerComponent,
  },
};
</script>

<template>
  <headerComponent></headerComponent>
  <mainComponent></mainComponent>
  <footerComponent></footerComponent>
</template>

<style scoped></style>
