<script setup>
import TheBanner from '../components/TheBanner.vue';
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
	<div>
		<LazyLoaded/>
	</div>
</template>


<style lang="scss" scoped>

</style>