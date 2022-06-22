<template>
  <div id="app">
    <TheHeader />
    <ComicsList />
    <TheFooter />
    <BannerSignUp />
  </div>
</template>

<script>
import TheHeader from './components/TheHeader.vue'
import ComicsList from './components/ComicsList.vue'
import TheFooter from './components/TheFooter.vue'
import BannerSignUp from './components/BannerSignUp.vue'

export default {
  name: 'App',
  components: {
    TheHeader,
    ComicsList,
    TheFooter,
    BannerSignUp
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
