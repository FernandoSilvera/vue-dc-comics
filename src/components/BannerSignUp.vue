<template>
  <section class="py-4">
    <div class="container">
      <div class="row justify-content-between align-items-center">
        <div class="col d-flex justify-content-start">
          <button class="text-uppercase my-btn">Sign-Up Now!</button>
        </div>

        <div class="col row">
          <div class="col d-flex align-items-center justify-content-end flex-grow-1 text-end">
            <h3 class="text-uppercase m-0">Follow Us</h3>
          </div>

          <div class="my-col flex-grow-0" v-for="(image, i) in images"  :key="i">
            <img :src="`img/footer-${image}.png`" alt="">
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'BannerSignUp',
  data() {
    return {
      images: ['facebook', 'twitter', 'youtube', 'pinterest', 'periscope']
    }
  }
}
</script>

<style lang="scss" scoped>
section {
    background-color: rgb(63, 63, 63);
}

.my-btn {
  color: white;
  background-color: rgb(63, 63, 63);
  padding: .8rem 1rem;
  border: 2px solid rgb(60, 92, 218);
}

.my-col {
    flex-basis: 20px;
    display: flex;
    align-items: center;
}

h3 {
    color: rgb(60, 92, 218);
}
</style>