<script lang="ts" setup>
	interface Props {
		title: string;
		pColor: string;
		pMarginBottom: string;
		btnName: string;
		bColor: string;
		bBorder: string;
		bBackgroundColor: string;
		bHeight: string;
		bWidth: string;
		bBoxShadow: string;
		icon: number;
	}

	const props = defineProps<Props>();
</script>

<template>
	<div class="flex flex-col">
		<p>{{ props.title }}</p>
		<button class="flex items-center justify-center" v-if="icon === 0">
			{{ props.btnName }}
		</button>
		<button class="flex items-center justify-center" v-else-if="icon === 1">
			<span class="material-icons-round mr-2 mt-[2px]"> add_shopping_cart </span>
			{{ props.btnName }}
		</button>
		<button class="flex items-center justify-center" v-else>
			{{ props.btnName }}
			<span class="material-icons-round ml-2 mt-[2px]"> add_shopping_cart </span>
		</button>
	</div>
</template>

<style scoped>
	p {
		color: v-bind('props.pColor');
		font-family: 'Ubuntu Mono', sans-serif;
		font-size: 12px;
		font-style: normal;
		font-weight: 400;
		height: 12px;
		line-height: normal;
		margin-bottom: v-bind('props.pMarginBottom');
	}
	button {
		background-color: v-bind('props.bBackgroundColor');
		border: v-bind('props.bBorder');
		border-radius: 6px;
		box-shadow: v-bind('props.bBoxShadow');
		color: v-bind('props.bColor');
		flex-shrink: 0;
		font-family: 'Noto Sans JP', sans-serif;
		font-size: 14px;
		font-style: normal;
		font-weight: 500;
		height: v-bind('props.bHeight');
		line-height: normal;
		text-align: center;
		width: v-bind('props.bWidth');
	}
</style>
