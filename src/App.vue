<template>
  <div id="app">
    <HelloWorld :msg="quotes"/>
    <quote :msg="quotes" @del_q="del_quote($event)" > </quote>
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
  },
  methods:{
    del_quote(index){
      this.quotes.splice(index,1);
    }
  }
}

</script>

<style>
#app {
 
}
</style>
