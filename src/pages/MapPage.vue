<template>
	<div>
		<LeafletMap />
	</div>
</template>

<script>
	import LeafletMap from "@/components/LeafletMap.vue";
	export default {
		components: {
			LeafletMap,
		},

		data() {
			return {
				name: "map",
			};
		},
		mounted() {},
	};
</script>

<style>
</style>

