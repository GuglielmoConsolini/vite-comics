<script>
import img1 from '../assets/buy-comics-digital-comics.png';
import img2 from '../assets/buy-comics-merchandise.png';
import img3 from '../assets/buy-comics-shop-locator.png';
import img4 from '../assets/buy-comics-subscriptions.png';
import img5 from '../assets/buy-dc-power-visa.svg';


import ComicList from './ComicList.vue';

export default {
  components: {
    ComicList
  },
  data() {
    return {
      options: [
        {
          text: "DIGITAL COMICS",
          img: img1,
        },
        {
          text: "DC MERCHANDISE",
          img: img2,
        },
        {
          text: "SUBSCRIPTION",
          img: img3,
        },
        {
          text: "SHOP LOCATIONS",
          img: img4,
        },
        {
          text: "DC POWER VISA",
          img: img5,
        },
      ],
    }
  }
}
</script>

<template>
  <div>
    <div class=" jumbotron position-relative container-fluid bg-dark p-5">
      <button type="button" class="pulsante btn btn-primary position-absolute">CURRENT SERIES</button>
    </div>

    <ComicList />
    
    <div class="container-fluid bg-primary p-5 d-flex">
      <div v-for="option in options" :key="option.text" class="option-item d-flex">
        <img :src="option.img" alt="">
        <p class="ms-2">{{ option.text }}</p>
      </div>
    </div>
  </div>
</template>

<style scoped>
.option-item {
  margin-right: 8rem;
}
img{
    width: 50px;
    height: 60px;
}
.jumbotron{
  background-image: url(../assets/jumbotron.jpg);
  height: 350px;
  background-size: cover;
  background-repeat: no-repeat;
}
.pulsante{
  bottom: -20px;
}
</style>