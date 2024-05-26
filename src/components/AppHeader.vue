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
                {
                    text: "GAMES",
                    url: "#contacts",
                },
                {
                    text: "GAMES",
                    url: "#contacts",
                },
                {
                    text: "GAMES",
                    url: "#contacts",
                }
            ],
        }
    }
}
</script>

<template>

   <div class="container-fluid bg-body pt-2 pb-2">
     <div class="row">
      <div class="col-6 text-center">
        <img src="../assets/dc-logo.png" alt="Bootstrap" width="60" height="60">
      </div>
      <div class="col-6 pt-3 text-center">
        <a class="me-3" v-for="link in links" :href="link.url">{{ link.text }}</a>
      </div>
     </div>
   </div>
</template>

<style scoped>
  a{
    text-decoration: none;
  }
</style>