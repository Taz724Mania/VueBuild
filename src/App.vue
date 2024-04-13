/* eslint-disable */
<template>
  <div id="app">
    <div>
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link> |
      <router-link to="/another">Another</router-link>
    </div>
    <HeaderVue />
    <router-view/>
    <FooterVue />
  </div>
</template>

<script>
import HeaderVue from "./components/Header.vue"
import FooterVue from "./components/Footer.vue"

export default {
  name: "App",
  components: {
    HeaderVue,
    FooterVue
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
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}
</style>
