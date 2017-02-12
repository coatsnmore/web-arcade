<template>
	<div>
		<h2>Arcade</h2>
		<p>Games and stuff.</p>
		<div id="scene"></div>
	</div>
</template>

<script>
  import Scene from '../webgl/Scene'

  export default {
    mounted: function () {
        this.scene = new Scene('scene', 600, 300)
        this.scene.tick();
    }
  }
</script async>