<template>
  <div class="card bg-dark border-0 my-card">
    <img :src="cardThumb" class="card-img-top" :alt="`${cardSeries} comic`">
    <div class="card-body px-0">
      <h5 class="card-title my-card-title">{{ cardSeries }}</h5>
    </div>
  </div>
</template>

<script>
  export default {
    name:"ComicCard",
    props: {
      cardThumb: String,
      cardPrice: String,
      cardSeries: String,
      cardType: String
    }
  }
</script>

<style lang="scss" scoped>
  .card-img-top {
    height: 200px;
    aspect-ratio: 1 / 1;
    object-fit: cover;
    object-position: top;
    border-radius: 0;
  }

  .my-card-title {
    color: white;
    font-size: 14px;
    text-align: left;
    text-transform: uppercase;
  }
</style>