<script setup>
	import LeftSide from './components/LeftSide.vue';
	import RightSide from './components/RightSide.vue';

	/* */
</script>

<template>
	<main class="flex min-h-screen">
		<LeftSide class="w-[237px]" />
		<RightSide class="w-[calc(100% - 237px)]" />
	</main>
</template>

<style scoped>
	/* */
</style>
