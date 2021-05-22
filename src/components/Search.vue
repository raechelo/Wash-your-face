<template>
  <input type="text" placeholder="Search">
</template>

<script>

export default {
  name: 'Search'
}

</script>

<style scoped lang="scss">
@import '../styles/variables.scss';

  input {
    border: $border;
    border-radius: $border-radius;
    display: block;
    margin: auto;
    font-size: 20px;
    padding: 3px;
  }

</style>