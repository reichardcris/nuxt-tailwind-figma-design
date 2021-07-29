<template>
	<div class="relative mt-24">
		<p class="title">Local Businesses Near You</p>
		<p class="mt-10 sub-title">Filter by</p>
		<div class="mt-5 grid grid-cols-4">
			<p class="filter-names" :class="{ active: true }">Ratings</p>
			<p class="filter-names">Reviews</p>
			<p class="filter-names">Name</p>
			<p class="filter-names">Nearest</p>
		</div>
	</div>
</template>

<style lang="scss" scoped>
	p {
		text-align: center;	
	}

 .title {
	font-style: normal;
	font-weight: bold;
	font-size: 35px;
	line-height: 42px;
	color: #38547B;
 }

	.filter-names {
		font-style: normal;
		font-weight: bold;
		font-size: 18px;
		line-height: 22px;
		color: #D6D6D6;
		cursor: pointer;
	}

	.active {
		text-decoration-line: underline;
		color: #38547B;
	}

 .sub-title {
	font-style: normal;
	font-weight: bold;
	font-size: 20px;
	line-height: 24px;
	color: #717171;
 }
</style>
