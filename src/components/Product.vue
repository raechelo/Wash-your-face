<template>
  <div class="background-outline"></div>
  <div class="product-outline">
      <div>
        <img src="{{ imgLink }}" alt="{{ imgDescription }}">
      </div>
      <div>
          <h3>{{ name }}</h3>
          <!-- put icon here with {{ containsMicroplastics }} -->
          <p>{{ description }}</p>
      </div>
  </div>
</template>

<script>

export default {
    name: 'Product',
    props: {
        imgLink: String,
        imgDescription: String,
        name: String,
        containsMicroplastics: Boolean,
        description: String,
    }

}
</script>

<style>

.background-outline {
    border: 10px solid black;
    transform: rotate(8deg);
}

</style>