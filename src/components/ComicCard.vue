<script>
export default {
    name: "ComicCard",
    props: ["fumetti"]
}
</script>

<template>
    <div class="cardsContainer">
        <div v-for="fumetto in fumetti" class="productCard">
             <img :src="fumetto.thumb" class="card-img-top" alt="...">
            <p class="card-text">{{ fumetto.series }}</p>
        </div>
     </div>
</template>

<style>
.cardsContainer{
display: flex;
flex-direction: row;
flex-wrap: wrap;
}
.productCard {
    width: 16.66%;
    padding: 1rem;
}
.productCard>img {
  width: 100%;
  aspect-ratio: 1;
  
}
</style>