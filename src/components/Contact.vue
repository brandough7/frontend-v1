<template>
	<div>
	<PageHeader :title="'CONTACT'"></PageHeader>

	<b-container class="py-5">
		<b-row align-h="center">
			<b-col cols="12" md="4">
				<b-form>
					<b-form-group label-for="lastname" label="Last name">
						<b-form-input id="lastname"  placeholder="Last name" size="sm"></b-form-input>
					</b-form-group>
					<b-form-group label-for="firstname" label="First name">
						<b-form-input id="firstname" placeholder="Last name" size="sm"></b-form-input>
					</b-form-group>
					<b-form-group
						id="input-group-1"
						label="Email address:"
						label-for="input-1"
						>
						<b-form-input
							id="input-1"
							type="email"
							required
							placeholder="Enter email"
							size="sm"
						></b-form-input>
					</b-form-group>
					<b-form-group label-for="mesage" label="Message">
						<b-form-textarea
							id="message"
							placeholder="Message"
							rows="4"
						></b-form-textarea>
					</b-form-group>
					<b-button type="submit" variant="info" align="left">Submit</b-button>
				</b-form>
			</b-col>
			<b-col cols="12" md="4" class="details py-3">
				<p class="text"><b-icon icon="globe" class="icons"></b-icon> 123 XYZ, Cebu City Philippines</p>
				<p class="text"><b-icon icon="telephone" class="icons"></b-icon> (032)1234567</p>
				<p class="text"><b-icon icon="envelope" class="icons"></b-icon> xyz@xyzcomp.com.ph</p>
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
	.details p{
		text-align: left;
		margin: 0 0 5px
	}

	.icons{
		color: #2c3e50;
		font-size: 20px;
	}
</style>