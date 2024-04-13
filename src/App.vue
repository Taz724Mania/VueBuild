<template>

<div>

  <h1>Hello World</h1>
  <h2>{{ cheese }}</h2>
  <GoodbyeWorld v-bind:cheese="cheese"/>
  <button v-on:click="handleClick"> Click Me </button>

</div>

</template>

<script>
import GoodbyeWorld from "./components/HelloWorld.vue"

export default {
  name: "App",
  data: function(){
    return {
      cheese: "gouda"
    }
  },
  components: {
    GoodbyeWorld
  },
  methods: {
    handleClick: function(){
      this.cheese = 'munster'
    }
  }
}
</script>

<style>

h1 {
  color: purple;
}

</style>