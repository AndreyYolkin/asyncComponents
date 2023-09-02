<script setup>
import TheBanner from './components/TheBanner.vue';
import {lazyLoadComponentIfVisible} from './utils'
const LazyLoaded = lazyLoadComponentIfVisible({
	componentLoader: () => import('~/components/HelloWorld.vue'),
	loadingComponent: TheBanner,
});
//props
//computed
//data
//methods
</script>
<template>
	<div >
		<div style="height: 1200px; width: 200px; background: linear-gradient(45deg, #cee, #eaa)">

		</div>
		<div style="height: 1200px; width: 200px; background: linear-gradient(45deg, #cee, #eaa)">

		</div>
		<div style="height: 1200px; width: 200px; background: linear-gradient(45deg, #cee, #eaa)">

		</div>
		<ClientOnly>	
			<LazyLoaded/>
		</ClientOnly>
	</div>
</template>


<style lang="scss" scoped>

</style>