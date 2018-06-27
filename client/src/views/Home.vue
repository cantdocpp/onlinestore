<template>
  <div class="home">
    <div class="uk-container">
      <Carousel/>
      <NewProduct></NewProduct>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import Carousel from '@/components/Carousel.vue'
import NewProduct from '@/components/NewProduct.vue'

export default {
  name: 'home',
  components: {
    Carousel,
    NewProduct
  }
}
</script>
