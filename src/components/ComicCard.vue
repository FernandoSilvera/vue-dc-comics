<template>
  <div class="card">
    <img :src="cardThumb" class="card-img-top" :alt="`${cardSeries} comic`">
    <div class="card-body">
      <h5 class="card-title">{{ cardSeries }}</h5>
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