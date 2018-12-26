<template>
  <div id="app">
    <HelloWorld msg=""/>
    <quote> </quote>
    <div class="bg-info container rounded p-2 text-center">
      <h2>Click on a quote to delete</h2>
    </div>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import quote from './components/quote.vue'

export default {
  name: 'app',
  components: {
    HelloWorld,
    quote
  }
}
</script>

<style>
#app {
 
}
</style>
