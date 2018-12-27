<template>
	<section class="container">
		
		<div class="m-1 d-flex">
			<div class="quote_container col-3 m-2" v-for="item in msg1" >
				<p>{{item}}
				</p>
			</div>
		</div>
	</section>
	
</template>
<script type="text/javascript">
	export default {
		props:{
			msg1:Array
		}
		
	}
	
</script>

<style type="text/css">
.quote_container{
	border: 1px solid blue;
}

</style>