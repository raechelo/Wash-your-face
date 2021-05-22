<template>
  <button v-on:click="onClick()">
    <icon icon="bars" class="icon"></icon>
  </button>
  <ul v-bind:class="{showMenu: showMenu}">
    <li>Home</li>
    <li>View All</li>
    <li>Search</li>
  </ul>
</template>

<script>

export default {
  name: 'Menu',
  data() {
    return {
      showMenu: false
    }
  },
  methods: {
    onClick() {
      this.showMenu = !this.showMenu
    }
  }
}
</script>
<style scoped lang="scss">
@import '../styles/variables';

  button {
    border: none;
    background-color: transparent;
    font-size: 30px;
    position: absolute;

    &:hover {
      cursor: pointer;
    }
  }

  ul {
    visibility: hidden;
    position: absolute;
    border: 5px solid black;
    padding: 0;
    top: 1.5rem;
    left: 1.5rem;

    li {
      padding: 10px 0;
      list-style-type: none;
      text-align: center;
      width: 120px;

      &:hover {
        background: $hover-gradient;
        cursor: pointer;
      }
    }
  }

  .showMenu {
    visibility: visible;
  }

</style>