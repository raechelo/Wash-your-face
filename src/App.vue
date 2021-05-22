<template>
  <Home />
</template>

<script>
import Home from './components/Home.vue'

export default {
  name: 'App',
  components: {
    Home
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Rammetto+One&family=Roboto&display=swap');


h1, h2 {
  font-family: 'Rammetto One', cursive;
  text-align: center;
  margin-top: 30px;
}

p, ul {
  font-family: 'Roboto', sans-serif;
}

</style>
