<template>
  <Header />
  <hr class="q-my-none"/>
  <router-view />
  <Footer />
</template>

<script lamg="ts">
import { defineComponent } from "@vue/runtime-core";
import Header from "./components/Layout/Header.vue";
import Footer from "./components/Layout/Footer.vue";
export default defineComponent({
  components: {
    Header,
    Footer
  }
});
</script>

<style lang="scss">
.screen-center {
  max-width: 1200px;
  margin: auto;
}
</style>
