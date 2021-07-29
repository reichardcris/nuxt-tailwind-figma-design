<template>
	<div class="filter-box flex flex-col justify-center justify-items-center justify-self-center items-center">
		<p class="text-title">Where do you need  the job done?</p>
		<!-- Input Filter -->
		<div class="w-ful mt-5">
				<form class="relative flex">
					<input class="filter-input focus:border-light-blue-500 focus:ring-1 focus:ring-light-blue-500 focus:outline-none" type="text" />
					<button class="filter-button rounded-full ml-6"> </button>
				</form>
		</div>
	</div>
</template>

<style lang="scss" scoped>
	.filter-box {
		width: 749px;
		height: 269px;
		background-color: #DEEDFF;
		border-radius: 50px;
	}

	.text-title {
		font-weight: bold;
		font-size: 35px;
		line-height: 42px;
		color: #38547B;
	}

	.filter-input {
		width: 443px;
		height: 65px;
		background: #FCFCFC;
		border-radius: 30px;
		font-size: 18px;
		line-height: 22px;
		padding-left: 16px;
		letter-spacing: 0.05em;
		color: #38547B;
	}

	.filter-button {
		width: 64px;
		height: 64px;
		background-image: url('~/assets/images/icons/arrow-right.svg');
	}
</style>