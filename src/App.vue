<template>
  <div id="app">
    <HelloWorld :msg="quotes"/>
    <quote :msg="quotes"> </quote>
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
  },
  data:function(){
    return{
     quotes:["this is the first quote"]
    }
  }
}

</script>

<style>
#app {
 
}
</style>
