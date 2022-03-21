<template>
  <div class="container-fluid">
    <div class="row">
      <div class="col-md-12 init">
        <img alt="Vue logo" src="./assets/bc.webp" style="width: 150px; ">
      </div>
      <div class="col-md-12 init">
        <HelloWorld msg="Welcome to My Portfolio App"/>
      </div>
    </div>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    HelloWorld
  }
}
</script>

<style>
.init {
  text-align: center;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
