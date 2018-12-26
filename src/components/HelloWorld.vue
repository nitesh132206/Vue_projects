<template>
  <div class="container">
    <div class="px-0">
      <!--     <h1>{{ msg }}</h1> -->

      <h1 class="my-2">Quotes Added</h1>
      <div class="my-2 bg-secondary">
        <div class="bar bg-info mb-5 d-block p-1" :style="{width:bar*10+'%'}" ><b class="ml-5">{{bar}}/10</b></div>
      </div>
      <form action="">
        <div class="form-group">
          <label class="form h1">Quote</label>
          <textarea id="quote_id" placeholder="enter your quote here .... " class="form-control"></textarea>
          <a href="" class="btn btn-danger my-2" :click="addquote">Add Quote</a>
        </div>
      </form>

    </div>
  </div>
</template>

<script>
  export default {
    name: 'HelloWorld',
    props: {
      msg: String
    },
    data:function(){
      return{
        bar:1,
        quotes:["first quote"]
      }
    },
    methods:{
      addquote:function(){
        quotes.push($("#quote_id").val())
      }

    }
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.bar{

  height: 30px;

}

</style>
