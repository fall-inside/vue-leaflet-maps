<template>
	<LeafletMap />
</template>

<script>
	import LeafletMap from "./components/LeafletMap.vue";

	export default {
		name: "App",
		components: {
			LeafletMap,
		},
	};
</script>

<style>
	#app {
		font-family: Avenir, Helvetica, Arial, sans-serif;
		-webkit-font-smoothing: antialiased;
		-moz-osx-font-smoothing: grayscale;
		text-align: center;
		color: #2c3e50;
		margin-top: 60px;
	}
</style>
