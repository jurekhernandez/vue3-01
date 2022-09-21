<script>
export default{
	
	data:()=>({
		contador:0,
	}),
	methods:{
		modificar(valor){
			this.contador += valor;
		},
		reset(){
			this.contador = 0;
		}
	}

};

</script>

<template>
	<div class="container">
		<img src="./assets/logo.svg" alt="Logo vue" width="125" height="125"/>
		<small>
			<h1>hola mundo desde vue 3</h1>
		</small>
		<hr>
		<h2>contador{{contador}}</h2>
		<button @click="modificar(+1);" >+1</button>
		<button @click="modificar(-1);">-1</button>
		<button @click="reset();">Reset</button>
	</div>
</template>

<style scoped>
	.container{
		text-align:center;
	}

	small{
		color:#666;
	}

	h1{
		font-weight: bolder;
	}
	h2{
		font-size: 2.5rem;
	}
	button{
		cursor: pointer;
		font-size: 1.5rem;
		margin: 0px 6px;
	}

	


</style>