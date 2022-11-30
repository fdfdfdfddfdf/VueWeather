<template>
  <HelloWorld>
  </HelloWorld>
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
#app {
display: flex;
align-items: center;
justify-content: center;
height: 100vh;
background: rgb(244, 123, 186);
background: linear-gradient(-25deg, rgba(244, 123, 186, 0.5) 20%, rgba(90, 95, 245, 0.5) 80%);
}
</style>
