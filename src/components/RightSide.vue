<script lang="ts" setup>
	import { reactive, ref } from 'vue';
	import ButtonLayout from './ButtonLayout.vue';

	const titles = ref({
		t01: '<Button />',
		t02: '&:hover, &:focus',
		t03: '<Button variant=”outline” />',
		t04: '<Button variant=”text” />',
		t05: '<Button disableShadow />',
		t06: '<Button disabled />',
		t07: '<Button variant=”text” disabled />',
		t08: '<Button startIcon=”local_grocery_store” />',
		t09: '<Button endIcon=”local_grocery_store” />',
		t10: '<Button size=”sm” />',
		t11: '<Button size=”md” />',
		t12: '<Button size=”lg” />',
		t13: '<Button color=”default” />',
		t14: '<Button color=”primary” />',
		t15: '<Button color=”secondary” />',
		t16: '<Button color=”danger” />',
		t17: ' ',
	});

	const btnNames = ref({
		n01: 'Default',
		n02: 'Disabled',
		n03: 'Secondary',
		n04: 'Danger',
	});

	const styles = reactive({
		b01: {
			pColor: '#333333',
			pMarginBottom: '12px',
			bColor: '#3F3F3F',
			bBorder: 'none',
			bBackgroundColor: '#e0e0e0',
			bHeight: '36px',
			bWidth: '81px',
			bBoxShadow: '0px 2px 3px 0px rgba(51, 51, 51, 0.2)',
		},
		b02: {
			pColor: '#828282',
			pMarginBottom: '12px',
			bColor: '#3F3F3F',
			bBorder: 'none',
			bBackgroundColor: '#AEAEAE',
			bHeight: '36px',
			bWidth: '81px',
			bBoxShadow: '0px 2px 3px 0px rgba(51, 51, 51, 0.20)',
		},
		b03: {
			pColor: '#333333',
			pMarginBottom: '12px',
			bColor: '#3D5AFE',
			bBorder: '1px solid #3D5AFE',
			bBackgroundColor: '#FFFFFF',
			bHeight: '36px',
			bWidth: '88px',
			bBoxShadow: 'none',
		},
		b04: {
			pColor: '#828282',
			pMarginBottom: '12px',
			bColor: '#3D5AFE',
			bBorder: '1px solid #3D5AFE',
			bBackgroundColor: 'rgba(41, 98, 255, 0.10)',
			bHeight: '36px',
			bWidth: '88px',
			bBoxShadow: 'none',
		},
		b05: {
			pColor: '#333333',
			pMarginBottom: '16px',
			bColor: '#3D5AFE',
			bBorder: 'none',
			bBackgroundColor: 'none',
			bHeight: '20px',
			bWidth: '49px',
			bBoxShadow: 'none',
		},
		b06: {
			pColor: '#828282',
			pMarginBottom: '12px',
			bColor: '#3D5AFE',
			bBorder: 'none',
			bBackgroundColor: 'rgba(41, 98, 255, 0.10)',
			bHeight: '36px',
			bWidth: '88px',
			bBoxShadow: 'none',
		},
		b07: {
			pColor: '#333333',
			pMarginBottom: '12px',
			bColor: '#FFFFFF',
			bBorder: 'none',
			bBackgroundColor: '#3D5AFE',
			bHeight: '36px',
			bWidth: '81px',
			bBoxShadow: 'none',
		},
		b08: {
			pColor: '#333333',
			pMarginBottom: '12px',
			bColor: '#9E9E9E',
			bBorder: 'none',
			bBackgroundColor: '#E0E0E0',
			bHeight: '36px',
			bWidth: '88px',
			bBoxShadow: 'none',
		},
		b09: {
			pColor: '#333333',
			pMarginBottom: '20px',
			bColor: '#9E9E9E',
			bBorder: 'none',
			bBackgroundColor: 'none',
			bHeight: '20px',
			bWidth: '62px',
			bBoxShadow: 'none',
		},
		b10: {
			pColor: '#333333',
			pMarginBottom: '12px',
			bColor: '#FFFFFF',
			bBorder: 'none',
			bBackgroundColor: '#2962FF',
			bHeight: '36px',
			bWidth: '105px',
			bBoxShadow: '0px 2px 3px 0px rgba(0, 49, 202, 0.20)',
		},
		b11: {
			pColor: '#333333',
			pMarginBottom: '12px',
			bColor: '#FFFFFF',
			bBorder: 'none',
			bBackgroundColor: '#2962FF',
			bHeight: '36px',
			bWidth: '105px',
			bBoxShadow: '0px 2px 3px 0px rgba(0, 49, 202, 0.20)',
		},
		b12: {
			pColor: '#333333',
			pMarginBottom: '17px',
			bColor: '#FFFFFF',
			bBorder: 'none',
			bBackgroundColor: '#2962FF',
			bHeight: '32px',
			bWidth: '73px',
			bBoxShadow: '0px 2px 3px 0px rgba(0, 49, 202, 0.20)',
		},
		b13: {
			pColor: '#333333',
			pMarginBottom: '15px',
			bColor: '#FFFFFF',
			bBorder: 'none',
			bBackgroundColor: '#2962FF',
			bHeight: '36px',
			bWidth: '81px',
			bBoxShadow: '0px 2px 3px 0px rgba(0, 49, 202, 0.20)',
		},
		b14: {
			pColor: '#333333',
			pMarginBottom: '12px',
			bColor: '#FFFFFF',
			bBorder: 'none',
			bBackgroundColor: '#2962FF',
			bHeight: '42px',
			bWidth: '93px',
			bBoxShadow: '0px 2px 3px 0px rgba(0, 49, 202, 0.20)',
		},
		b15: {
			pColor: '#333333',
			pMarginBottom: '12px',
			bColor: '#3F3F3F',
			bBorder: 'none',
			bBackgroundColor: '#E0E0E0',
			bHeight: '36px',
			bWidth: '81px',
			bBoxShadow: '0px 2px 3px 0px rgba(51, 51, 51, 0.20)',
		},
		b16: {
			pColor: '#333333',
			pMarginBottom: '12px',
			bColor: '#FFFFFF',
			bBorder: 'none',
			bBackgroundColor: '#2962FF',
			bHeight: '36px',
			bWidth: '81px',
			bBoxShadow: '0px 2px 3px 0px rgba(0, 49, 202, 0.20)',
		},
		b17: {
			pColor: '#333333',
			pMarginBottom: '12px',
			bColor: '#FFFFFF',
			bBorder: 'none',
			bBackgroundColor: '#455A64',
			bHeight: '36px',
			bWidth: '104px',
			bBoxShadow: '0px 2px 3px 0px rgba(69, 90, 100, 0.20)',
		},
		b18: {
			pColor: '#333333',
			pMarginBottom: '12px',
			bColor: '#FFFFFF',
			bBorder: 'none',
			bBackgroundColor: '#D32F2F',
			bHeight: '36px',
			bWidth: '81px',
			bBoxShadow: '0px 2px 3px 0px rgba(211, 47, 47, 0.20)',
		},
		b19: {
			pColor: '#828282',
			pMarginBottom: '12px',
			bColor: '#3F3F3F',
			bBorder: 'none',
			bBackgroundColor: '#AEAEAE',
			bHeight: '36px',
			bWidth: '81px',
			bBoxShadow: '0px 2px 3px 0px rgba(51, 51, 51, 0.20)',
		},
		b20: {
			pColor: 'none',
			pMarginBottom: '12px',
			bColor: '#FFFFFF',
			bBorder: 'none',
			bBackgroundColor: '#0039CB',
			bHeight: '36px',
			bWidth: '81px',
			bBoxShadow: '0px 2px 3px 0px rgba(41, 98, 255, 0.20)',
		},
		b21: {
			pColor: 'none',
			pMarginBottom: '12px',
			bColor: '#FFFFFF',
			bBorder: 'none',
			bBackgroundColor: '#1C313A',
			bHeight: '36px',
			bWidth: '104px',
			bBoxShadow: '0px 2px 3px 0px rgba(69, 90, 100, 0.20)',
		},
		b22: {
			pColor: 'none',
			pMarginBottom: '12px',
			bColor: '#FFFFFF',
			bBorder: 'none',
			bBackgroundColor: '#9A0007',
			bHeight: '36px',
			bWidth: '81px',
			bBoxShadow: '0px 2px 3px 0px rgba(211, 47, 47, 0.20)',
		},
	});
</script>

<template>
	<div class="pl-[83px] bg-[#FFFFFF]">
		<h2>Buttons</h2>
		<div class="flex mb-[45px]">
			<ButtonLayout
				:title="titles.t01"
				:pColor="styles.b01.pColor"
				:pMarginBottom="styles.b01.pMarginBottom"
				:btnName="btnNames.n01"
				:bColor="styles.b01.bBorder"
				:bBorder="styles.b01.bBorder"
				:bBackgroundColor="styles.b01.bBackgroundColor"
				:bHeight="styles.b01.bHeight"
				:bWidth="styles.b01.bWidth"
				:bBoxShadow="styles.b01.bBoxShadow"
				:icon="0"
				class="mr-[155px]"
			/>
			<ButtonLayout
				:title="titles.t02"
				:pColor="styles.b02.pColor"
				:pMarginBottom="styles.b02.pMarginBottom"
				:btnName="btnNames.n01"
				:bColor="styles.b02.bColor"
				:bBorder="styles.b02.bBorder"
				:bBackgroundColor="styles.b02.bBackgroundColor"
				:bHeight="styles.b02.bHeight"
				:bWidth="styles.b02.bWidth"
				:bBoxShadow="styles.b02.bBoxShadow"
				:icon="0"
			/>
		</div>
		<div class="flex mb-[45px]">
			<ButtonLayout
				:title="titles.t03"
				:pColor="styles.b03.pColor"
				:pMarginBottom="styles.b03.pMarginBottom"
				:btnName="btnNames.n01"
				:bColor="styles.b03.bColor"
				:bBorder="styles.b03.bBorder"
				:bBackgroundColor="styles.b03.bBackgroundColor"
				:bHeight="styles.b03.bHeight"
				:bWidth="styles.b03.bWidth"
				:bBoxShadow="styles.b03.bBoxShadow"
				:icon="0"
				class="mr-[68px]"
			/>
			<ButtonLayout
				:title="titles.t02"
				:pColor="styles.b04.pColor"
				:pMarginBottom="styles.b04.pMarginBottom"
				:btnName="btnNames.n01"
				:bColor="styles.b04.bColor"
				:bBorder="styles.b04.bBorder"
				:bBackgroundColor="styles.b04.bBackgroundColor"
				:bHeight="styles.b04.bHeight"
				:bWidth="styles.b04.bWidth"
				:bBoxShadow="styles.b04.bBoxShadow"
				:icon="0"
			/>
		</div>
		<div class="flex mb-[45px]">
			<ButtonLayout
				:title="titles.t04"
				:pColor="styles.b05.pColor"
				:pMarginBottom="styles.b05.pMarginBottom"
				:btnName="btnNames.n01"
				:bColor="styles.b05.bColor"
				:bBorder="styles.b05.bBorder"
				:bBackgroundColor="styles.b05.bBackgroundColor"
				:bHeight="styles.b05.bHeight"
				:bWidth="styles.b05.bWidth"
				:bBoxShadow="styles.b05.bBoxShadow"
				:icon="0"
				class="mr-[86px]"
			/>
			<ButtonLayout
				:title="titles.t02"
				:pColor="styles.b06.pColor"
				:pMarginBottom="styles.b06.pMarginBottom"
				:btnName="btnNames.n01"
				:bColor="styles.b06.bColor"
				:bBorder="styles.b06.bBorder"
				:bBackgroundColor="styles.b06.bBackgroundColor"
				:bHeight="styles.b06.bHeight"
				:bWidth="styles.b06.bWidth"
				:bBoxShadow="styles.b06.bBoxShadow"
				:icon="0"
			/>
		</div>
		<div class="mb-[45px]">
			<ButtonLayout
				:title="titles.t05"
				:pColor="styles.b07.pColor"
				:pMarginBottom="styles.b07.pMarginBottom"
				:btnName="btnNames.n01"
				:bColor="styles.b07.bColor"
				:bBorder="styles.b07.bBorder"
				:bBackgroundColor="styles.b07.bBackgroundColor"
				:bHeight="styles.b07.bHeight"
				:bWidth="styles.b07.bWidth"
				:bBoxShadow="styles.b07.bBoxShadow"
				:icon="0"
			/>
		</div>
		<div class="flex mb-[45px]">
			<ButtonLayout
				:title="titles.t06"
				:pColor="styles.b08.pColor"
				:pMarginBottom="styles.b08.pMarginBottom"
				:btnName="btnNames.n02"
				:bColor="styles.b08.bColor"
				:bBorder="styles.b08.bBorder"
				:bBackgroundColor="styles.b08.bBackgroundColor"
				:bHeight="styles.b08.bHeight"
				:bWidth="styles.b08.bWidth"
				:bBoxShadow="styles.b08.bBoxShadow"
				:icon="0"
				class="mr-[125px]"
			/>
			<ButtonLayout
				:title="titles.t07"
				:pColor="styles.b09.pColor"
				:pMarginBottom="styles.b09.pMarginBottom"
				:btnName="btnNames.n02"
				:bColor="styles.b09.bColor"
				:bBorder="styles.b09.bBorder"
				:bBackgroundColor="styles.b09.bBackgroundColor"
				:bHeight="styles.b09.bHeight"
				:bWidth="styles.b09.bWidth"
				:bBoxShadow="styles.b09.bBoxShadow"
				:icon="0"
			/>
		</div>
		<div class="flex mb-[45px]">
			<ButtonLayout
				:title="titles.t08"
				:pColor="styles.b10.pColor"
				:pMarginBottom="styles.b10.pMarginBottom"
				:btnName="btnNames.n01"
				:bColor="styles.b10.bColor"
				:bBorder="styles.b10.bBorder"
				:bBackgroundColor="styles.b10.bBackgroundColor"
				:bHeight="styles.b10.bHeight"
				:bWidth="styles.b10.bWidth"
				:bBoxShadow="styles.b10.bBoxShadow"
				:icon="1"
				class="mr-[80px]"
			/>
			<ButtonLayout
				:title="titles.t09"
				:pColor="styles.b11.pColor"
				:pMarginBottom="styles.b11.pMarginBottom"
				:btnName="btnNames.n01"
				:bColor="styles.b11.bColor"
				:bBorder="styles.b11.bBorder"
				:bBackgroundColor="styles.b11.bBackgroundColor"
				:bHeight="styles.b11.bHeight"
				:bWidth="styles.b11.bWidth"
				:bBoxShadow="styles.b11.bBoxShadow"
				:icon="2"
			/>
		</div>
		<div class="flex mb-[45px]">
			<ButtonLayout
				:title="titles.t10"
				:pColor="styles.b12.pColor"
				:pMarginBottom="styles.b12.pMarginBottom"
				:btnName="btnNames.n01"
				:bColor="styles.b12.bColor"
				:bBorder="styles.b12.bBorder"
				:bBackgroundColor="styles.b12.bBackgroundColor"
				:bHeight="styles.b12.bHeight"
				:bWidth="styles.b12.bWidth"
				:bBoxShadow="styles.b12.bBoxShadow"
				:icon="0"
				class="mr-[84px]"
			/>
			<ButtonLayout
				:title="titles.t11"
				:pColor="styles.b13.pColor"
				:pMarginBottom="styles.b13.pMarginBottom"
				:btnName="btnNames.n01"
				:bColor="styles.b13.bColor"
				:bBorder="styles.b13.bBorder"
				:bBackgroundColor="styles.b13.bBackgroundColor"
				:bHeight="styles.b13.bHeight"
				:bWidth="styles.b13.bWidth"
				:bBoxShadow="styles.b13.bBoxShadow"
				:icon="0"
				class="mr-[88px]"
			/>
			<ButtonLayout
				:title="titles.t12"
				:pColor="styles.b14.pColor"
				:pMarginBottom="styles.b14.pMarginBottom"
				:btnName="btnNames.n01"
				:bColor="styles.b14.bColor"
				:bBorder="styles.b14.bBorder"
				:bBackgroundColor="styles.b14.bBackgroundColor"
				:bHeight="styles.b14.bHeight"
				:bWidth="styles.b14.bWidth"
				:bBoxShadow="styles.b14.bBoxShadow"
				:icon="0"
			/>
		</div>
		<div class="flex mb-[45px]">
			<ButtonLayout
				:title="titles.t13"
				:pColor="styles.b15.pColor"
				:pMarginBottom="styles.b15.pMarginBottom"
				:btnName="btnNames.n01"
				:bColor="styles.b15.bColor"
				:bBorder="styles.b15.bBorder"
				:bBackgroundColor="styles.b15.bBackgroundColor"
				:bHeight="styles.b15.bHeight"
				:bWidth="styles.b15.bWidth"
				:bBoxShadow="styles.b15.bBoxShadow"
				:icon="0"
				class="mr-[45px]"
			/>
			<ButtonLayout
				:title="titles.t14"
				:pColor="styles.b16.pColor"
				:pMarginBottom="styles.b16.pMarginBottom"
				:btnName="btnNames.n01"
				:bColor="styles.b16.bColor"
				:bBorder="styles.b16.bBorder"
				:bBackgroundColor="styles.b16.bBackgroundColor"
				:bHeight="styles.b16.bHeight"
				:bWidth="styles.b16.bWidth"
				:bBoxShadow="styles.b16.bBoxShadow"
				:icon="0"
				class="mr-[52px]"
			/>
			<ButtonLayout
				:title="titles.t15"
				:pColor="styles.b17.pColor"
				:pMarginBottom="styles.b17.pMarginBottom"
				:btnName="btnNames.n03"
				:bColor="styles.b17.bColor"
				:bBorder="styles.b17.bBorder"
				:bBackgroundColor="styles.b17.bBackgroundColor"
				:bHeight="styles.b17.bHeight"
				:bWidth="styles.b17.bWidth"
				:bBoxShadow="styles.b17.bBoxShadow"
				:icon="0"
				class="mr-[72px]"
			/>
			<ButtonLayout
				:title="titles.t16"
				:pColor="styles.b18.pColor"
				:pMarginBottom="styles.b18.pMarginBottom"
				:btnName="btnNames.n04"
				:bColor="styles.b18.bColor"
				:bBorder="styles.b18.bBorder"
				:bBackgroundColor="styles.b18.bBackgroundColor"
				:bHeight="styles.b18.bHeight"
				:bWidth="styles.b18.bWidth"
				:bBoxShadow="styles.b18.bBoxShadow"
				:icon="0"
			/>
		</div>
		<div class="flex mb-[52px]">
			<ButtonLayout
				:title="titles.t02"
				:pColor="styles.b19.pColor"
				:pMarginBottom="styles.b19.pMarginBottom"
				:btnName="btnNames.n01"
				:bColor="styles.b19.bColor"
				:bBorder="styles.b19.bBorder"
				:bBackgroundColor="styles.b19.bBackgroundColor"
				:bHeight="styles.b19.bHeight"
				:bWidth="styles.b19.bWidth"
				:bBoxShadow="styles.b19.bBoxShadow"
				:icon="0"
				class="mr-[103px]"
			/>
			<ButtonLayout
				:title="titles.t17"
				:pColor="styles.b20.pColor"
				:pMarginBottom="styles.b20.pMarginBottom"
				:btnName="btnNames.n01"
				:bColor="styles.b20.bColor"
				:bBorder="styles.b20.bBorder"
				:bBackgroundColor="styles.b20.bBackgroundColor"
				:bHeight="styles.b20.bHeight"
				:bWidth="styles.b20.bWidth"
				:bBoxShadow="styles.b20.bBoxShadow"
				:icon="0"
				class="mr-[127px]"
			/>
			<ButtonLayout
				:title="titles.t17"
				:pColor="styles.b21.pColor"
				:pMarginBottom="styles.b21.pMarginBottom"
				:btnName="btnNames.n03"
				:bColor="styles.b21.bColor"
				:bBorder="styles.b21.bBorder"
				:bBackgroundColor="styles.b21.bBackgroundColor"
				:bHeight="styles.b21.bHeight"
				:bWidth="styles.b21.bWidth"
				:bBoxShadow="styles.b21.bBoxShadow"
				:icon="0"
				class="mr-[136px]"
			/>
			<ButtonLayout
				:title="titles.t17"
				:pColor="styles.b22.pColor"
				:pMarginBottom="styles.b22.pMarginBottom"
				:btnName="btnNames.n04"
				:bColor="styles.b22.bColor"
				:bBorder="styles.b22.bBorder"
				:bBackgroundColor="styles.b22.bBackgroundColor"
				:bHeight="styles.b22.bHeight"
				:bWidth="styles.b22.bWidth"
				:bBoxShadow="styles.b22.bBoxShadow"
				:icon="0"
			/>
		</div>
		<p class="icons">Icons: https://material.io/resources/icons/?style=round</p>
		<p class="created">
			created by
			<a href="https://devchallenges.io/portfolio/drfcozapata"
				><span>drfcozapata</span></a
			>
			- devChallenges.io
		</p>
	</div>
</template>

<style scoped>
	h2 {
		font-family: Poppins, sans-serif;
		color: #4f4f4f;
		font-size: 24px;
		font-weight: 500;
		height: 36px;
		margin: 53px 0 28px 1px;
	}
</style>
