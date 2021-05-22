<template>
  <Menu />
  <Search />
  <h1>Wash Your Face!</h1>
  <h2>And Save the Oceans</h2>
  <div class="container">
    <div class="inner-container">
      <p>some text for placeholder</p>
    </div> 
  </div>

  <!-- <div  v-for="product in products" v-bind:key="product.uuid">
    <Product 
            [name]="product.name"
            [img-link]="product.imgLink"
            [img-description]="product.imgDescription"
            [contains-microplastics]="product.containsMicroplastics"
            [description]="product.description" 
            />
  </div> -->
</template>

<script>
// import Product from './Product.vue';
import Search from './Search';
import Menu from './Menu';

export default {
  name: 'Home',
  components: {
    // Product,
    Search,
    Menu
  },
  props: ['products']
}

// const products = [
//   { name: 'Neutrogena Pink Grapefruit Foaming Scrub',
//   imgLink: 'https://m.media-amazon.com/images/I/41jrUg6EvIL.jpg',
//   imgDescription: 'Neutrogena Pink Grapefruit Foaming Scrub picture',
//   description: 'some description here',
//   containsMicroplastics: false}
// ]

</script>


<style scoped lang="scss">
@import '../styles/variables';
h1 {
  margin: 15px auto 10px auto;
}

h2 {
  margin: 0 auto;
  font-size: 20px;
}

.container {
  border: $border;
  width: 40%;
  height: 40%;
  margin: 2rem auto;
  transform: rotate(352deg);
}

.inner-container {
  border: 7px solid transparent;
  border-image-slice: 1;
  border-image-source: $gradient;
  transform: rotate(8deg);
  background: white;
  height: 40vh;
}
</style>
