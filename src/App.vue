<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';

export default {
  components: {
    AppHeader,
    AppMain,
    AppFooter
  },
  data() {
    return {
      autore: "Luca Lambiase"
    }
  },
  methods: {
    welcome() {
      console.log("Benvenuto nell'applicazione di La Molisana, sviluppata da ", this.autore);
    }
  },
  mounted() {
    this.welcome();
  }
}
</script>

<template>
      <AppHeader />
      <AppMain />
      <AppFooter />
      <AppEnd />

</template>


