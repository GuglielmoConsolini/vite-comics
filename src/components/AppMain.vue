<!-- <script>
  export default {
    data() {
        return {
            options: [
                {
                    text: "DIGITAL COMICS",
                    img: "../assets/buy-comics-digital-comics.png",
                },
                {
                    text: "DC MERCHANDISE",
                    img: "../assets/buy-comics-merchandise.png",
                },
                {
                    text: "SUBSCRIPTION",
                    img: "../assets/buy-comics-shop-locator.png",
                },
                {
                    text: "SHOP LOCATIONS",
                    img: "../assets/buy-comics-subscriptions.png",
                },
                {
                    text: "DC POWER VISA",
                    img: "../assets/buy-dc-power-visa.svg",
                },
            ],
        }
    }
}
</script>

<template>
  <div class="container-fluid bg-dark p-5">
    <h1>CONTENT GOES HERE</h1>
  </div>
  <div class="container-fluid bg-primary p-5 d-flex">
    <div v-for="option in options">
        <img :src="option.img"  alt="">
        <p>{{ option.text }}</p>
    </div>
  </div>
</template>

<style>

</style> -->
<script>
import img1 from '../assets/buy-comics-digital-comics.png';
import img2 from '../assets/buy-comics-merchandise.png';
import img3 from '../assets/buy-comics-shop-locator.png';
import img4 from '../assets/buy-comics-subscriptions.png';
import img5 from '../assets/buy-dc-power-visa.svg';

export default {
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
    <div class="container-fluid bg-dark p-5">
      <h1>CONTENT GOES HERE</h1>
    </div>
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
  margin-right: 10rem;
}
img{
    width: 50px;
    height: 60px;
}
</style>