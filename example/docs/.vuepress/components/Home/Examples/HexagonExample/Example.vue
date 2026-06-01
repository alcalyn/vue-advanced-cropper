<template>
	<Cropper
		class="hexagon-example"
		:src="require('./assets/image.jpg')"
		:stencil-component="stencil"
		:stencil-props="{ aspectRatio: 2 / Math.sqrt(3) }"
	/>
</template>

<script>
import { Cropper, HexagonStencil } from 'vue-advanced-cropper';

export default {
	name: 'HexagonExample',
	components: {
		Cropper,
	},
	data() {
		return {
			stencil: HexagonStencil,
		};
	},
};
</script>

<style lang="scss">
.hexagon-example {
	background: black;
}
</style>
