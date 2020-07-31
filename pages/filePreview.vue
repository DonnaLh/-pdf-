<template>
	<view>
		<web-view :src="url"></web-view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				url: '',
			};
		},
		onLoad(params){
			let {url} = params
			this.url = `/hybrid/html/pdf.html?url=${url}`
		},
		onBackPress(){}
	}
</script>

<style>
</style>
