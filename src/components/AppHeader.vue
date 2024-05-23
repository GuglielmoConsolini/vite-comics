<script>
  export default {
    data() {
        return {
            links: [
                {
                    text: "CHARACTERS",
                    url: "#home",
                },
                {
                    text: "COMICS",
                    url: "#products",
                },
                {
                    text: "MOVIES",
                    url: "#who",
                },
                {
                    text: "TV",
                    url: "#contacts",
                },
                {
                    text: "GAMES",
                    url: "#contacts",
                },
            ],
        }
    }
}
</script>

<template>
<nav class="navbar bg-body-tertiary">
  <div class="container">
    <a class="navbar-brand" href="#">
      <img src="../assets/dc-logo.png" alt="Bootstrap" width="50" height="50">
    </a>
    <a v-for="link in links" :href="link.url">{{ link.text }}</a>
  </div>
</nav>
</template>

<style scoped>
  a{
    text-decoration: none;
  }
</style>