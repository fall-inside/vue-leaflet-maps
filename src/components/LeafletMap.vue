<template>
	<div
		class="leaflet-map"
		id="map"
	>
	</div>
</template>

<script>
	import "leaflet/dist/leaflet.css";
	import L from "leaflet";

	export default {
		name: "LeafletMap",
		data() {
			return {
				map: null,
			};
		},
		computed: {
			mapMarkers: function () {
				return this.markers;
			},
		},
		mounted() {
			this.map = L.map("map").setView([51.959, -8.623], 4);
			L.tileLayer("https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png", {
				maxZoom: 8,
			}).addTo(this.map);
			console.debug("map created");
		},
		methods: {},
	};
</script>

<style scoped>
	#map {
		width: 100vw;
		height: 100vh;
	}
</style>
