<template>
	<div>
		<PageHeader :title="'ABOUT US'"></PageHeader>

		<b-container class="py-5">
			<b-row>
				<b-col cols="12">
					<p class="text">"Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum."</p>
				</b-col>
				<b-col cols="12" md="6">
					<b-img class="py-3" src="https://picsum.photos/id/1/367/267" rounded fluid></b-img>
				</b-col>
				<b-col cols="12" md="6">
					<p class="text-left py-3 text">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam facilisis dignissim leo, ut aliquam metus. Nunc sagittis est felis, maximus bibendum erat feugiat sit amet. Mauris luctus elementum dolor, et lobortis odio porttitor sit amet. Sed ut mi quis turpis maximus varius. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum eget venenatis turpis. Suspendisse at suscipit erat, sit amet lobortis tellus. Cras consequat diam metus, nec accumsan tortor vulputate et. Mauris tempus lectus lobortis, efficitur urna eget, fermentum augue. Mauris facilisis odio sit amet vulputate posuere. Nullam imperdiet, ipsum non bibendum convallis, tortor nulla vestibulum ipsum, quis imperdiet nisl justo at dolor. Ut at elementum magna. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas.
						<br><br>	
					Duis sed semper magna, a egestas ex. Curabitur ultrices urna neque, ac rhoncus dui consectetur eu. Maecenas et lacinia nibh, sed sollicitudin sem. Sed molestie lacinia sapien, in accumsan diam scelerisque in. Integer ut pretium libero. Proin finibus est velit, in accumsan nisl rhoncus ac. Quisque dictum lectus quis mi rhoncus, id pulvinar ipsum efficitur. Etiam molestie mauris at lorem bibendum placerat. In condimentum sodales cursus.

					</p>
				</b-col>
			</b-row>
		</b-container>
	</div>
</template>
<script>
	import PageHeader from '@/components/PageHeader.vue'

	export default{
		components:{
			PageHeader
		}
	}
</script>
<style scoped>
	

	.img_header{
		object-fit: cover !important;
		width: 100%;
    height: 100px !important;
	}

	.wrapper {
		position: relative;
		text-align: center;
		color: white;
	}

	.centered {
		position: absolute;
		top: 50%;
		left: 50%;
		transform: translate(-50%, -50%);

		animation-duration: 3s;
		animation-name: slidein;
		animation-iteration-count: infinite;
	}

	

	
</style>