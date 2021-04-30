<template>
  <q-layout view="lHh lpR lFf">
    <Header />
    <hr class="q-my-none" />
    <q-page-container>
      <router-view />
    </q-page-container>
    <Footer />
  </q-layout>
</template>

<script lamg="ts">
import { defineComponent } from "vue";
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
