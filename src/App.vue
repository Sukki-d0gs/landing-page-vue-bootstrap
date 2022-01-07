<template>
  <Navbar />
  <Product_preview />
  <hr>
  <div id="pricing">
    <Cards />
  </div>
  <hr>
  <Footer />
</template>

<script>
import Navbar from './components/Navbar.vue'
import Product_preview from './components/Product_preview.vue'
import Cards from './components/Cards.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Navbar,
    Product_preview,
    Cards,
    Footer
  }
}
</script>

<style scoped>
  #pricing {
    padding-top: 10%;
    padding-bottom: 10%;
  }
</style>