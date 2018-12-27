<template>
  <div id="app">
    <HelloWorld :msg="quotes" @add_quote="quotes.unshift($event)"/>
    <quote :msg1="quotes" > </quote>
    <div class="bg-info container rounded p-2 text-center">
      <h2>Click on a quote to delete</h2>
    </div>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import quote from './components/quote.vue'

export default {
  components: {
    HelloWorld,
    quote
  },
  data:function(){
    return{
    quotes:["this is the first quote"]
    }
  },
  // methods:{
  //   addquote:function(){
  //       //quotes.shift($("#quote_id").val())
        
  //       this.quotes.push($event)
  //       alert(this.quotes)
      
  // }
}

</script>

<style>
#app {
 
}
</style>
