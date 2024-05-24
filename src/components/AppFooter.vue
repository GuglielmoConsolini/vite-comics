<script>

  import AppEnd from './AppEnd.vue';

  export default {
  name: 'ParentComponent',
  components: {
    AppEnd
  }, 

  data() {
    return {
      liste: [
        {
          text: "DC COMICS",
          img: [
            'comics',
            'comics',
            'comics',
            'comics',
            'comics',
            'comics'
          ]
        },
        {
          text: "SHOP",
          img: [
            'comics',
            'comics',
            'comics',
            'comics',
            'comics',
            'comics'
          ]
        },
        {
          text: "DC",
          img: [
            'comics',
            'comics',
          ]
        },
        {
          text: "SHOP LOCATIONS",
          img: [
            'comics',
            'comics',
            'comics',
            
          ]
        },
        {
          text: "SITES",
          img: [
            'comics',
            'comics',
            'comics',
            
          ]
        },
      ],
    }
  }
}
</script>

<template>
  <div class="footer-container">
    <div class="sfondo-box container-fluid d-flex p-4">
      <div v-for="(lista, index) in liste" :key="index" class="list-container me-5">
        <h5 class="ms-4">{{ lista.text }}</h5>
        <ul>
          <li v-for="(img, imgIndex) in lista.img" :key="imgIndex">{{ img }}</li>
        </ul>
      </div>
    </div>
    <img src="../assets/dc-logo-bg.png" alt="" class="background-image">
  </div>
  <AppEnd />
</template>

<style scoped>
.footer-container {
  position: relative;
  height: 350px; 
  overflow: hidden; 
}
.sfondo-box{
    background-image: url(../assets/footer-bg.jpg);
    background-size: cover;
    background-repeat: no-repeat;
    height: 100%;
    position: relative;
}
.background-image {
  position: absolute; 
  top: -100px; 
  right: 50px; 
}
li{
  list-style: none;
}
</style>