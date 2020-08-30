<template>
	<div class="wrapper">
		<img class="img_header" src="https://images.unsplash.com/photo-1461749280684-dccba630e2f6?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=750&q=80"/>
		<h2 class="centered text-white">{{ title }}</h2>
	</div>
</template>
<script>
	export default{
		props: {
			title: String
		}
	}
</script>
<style scoped>
	.img_header{
		object-fit: cover !important;
		width: 100%;
    height: 100px !important;
		-webkit-filter: blur(1px);
	}

	.wrapper {
		position: relative;
		text-align: center;
		color: white;
	}

	.centered {
		position: absolute;
		top: 50%;
		right: 80px;
		transform: translate(-50%, -50%);
		border: 3px solid #f1f1f1;
		padding: 10px;
		font-size: 3vh;
	}

	@media (max-width:481px)  {
		.centered{
			right: 0px;
			left: 50% !important;
		}

		.img_header{
			-webkit-filter: blur(2px);
		}

	}
</style>