<template>
  <HeaderComponent/>
  <FooterComponent/>
</template>

<script>
import HeaderComponent from './components/header.vue'
import FooterComponent from './components/footer.vue'

export default {
  name: 'App',
  components: {
    HeaderComponent,
    FooterComponent,
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
