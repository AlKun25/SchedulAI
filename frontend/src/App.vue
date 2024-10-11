<template>
  <div id="app">
    <HeaderPart />
    <MainContent />
    <FooterPart />
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import HeaderPart from "./components/HeaderPart.vue";
import MainContent from "./components/MainContent.vue";
import FooterPart from "./components/FooterPart.vue";

export default defineComponent({
  name: "App",
  components: {
    HeaderPart,
    MainContent,
    FooterPart,
  },
});
</script>

<style>
#app {
  display: grid;
  grid-template-rows: auto 1fr auto;
  min-height: 100vh;
}
</style>
