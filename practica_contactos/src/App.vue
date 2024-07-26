<template>
  <nav>
    <!-- -->
    <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link>|
    <router-link to="/parqueo">Parqueo</router-link>
  </nav>


  <div id="app">
    <ParqueoView />
  </div>

  <!-- <router-view/> -->
</template>

<script>
import ParqueoView from './views/ParqueoView.vue'

export default {
  components: {
    ParqueoView
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

nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
