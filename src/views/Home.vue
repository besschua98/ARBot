<template>
  <div class="home">
    <!-- <img src="../assets/logo.png"> -->
		<a-scene embedded arjs="debugUIEnabled:false; sourceType: webcam; detectionMode: mono; maxDetectionRate: 15;" vr-mode-ui="enabled: false">
			<a-marker preset='custom' url='assets/logo_marker.patt' changeMatrixMode='modelViewMatrix'></a-marker>
			<a-entity camera></a-entity>
		</a-scene>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';
@Component({
  components: {},
})
export default class Home extends Vue {}
</script>
