<template>
	<section class="container">
		
		<div class="m-1 row justify-content-around" >
			<div class="quote_container col-3 m-2" v-for="(items,index) in msg" @click="$emit('del_q',index)"  >
				<p>{{items}}
				</p>
			</div>
		</div>
	</section>
	
</template>
<script type="text/javascript">
	export default {
		props:{
			msg:Array
		}
		
	}
	
</script>

<style type="text/css">
.quote_container{
	border: 1px solid blue;
	border-radius: 7px;
	
	
}
div.quote_container:hover{
	background-color: #C2DFE3;
}



</style>