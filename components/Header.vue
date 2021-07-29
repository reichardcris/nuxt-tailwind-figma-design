<template>
  <div class="navbar flex flex-row justify-between">
		
		<!-- Logo section -->
		<NuxtLink to="/">
			<img :src="require('~/assets/images/logo.svg')" />
		</NuxtLink>
		
		<!-- User Avatar Section -->
		<div class="flex flex-row box-border items-center">
			
			<!-- Avatar -->
			<div class="avatar rounded-full mr-5 flex flex-row justify-center justify-items-center items-center">
				<span>S</span>
			</div>

			<!-- User Name -->
			<div class="user-name mr-12">
				Samantha
			</div>
			
			<!-- Right Search Bar -->
			<div class="w-ful">
				<form class="relative">
					<img
						:src="require('~/assets/images/icons/search.svg')"
						width="15"
						height="15"
						fill="currentColor"
						class="absolute right-3 top-1/2 transform -translate-y-1/2 text-gray-400" 
					/>
					<input 
						class="search-bar focus:border-light-blue-500 focus:ring-1 focus:ring-light-blue-500 focus:outline-none text-sm text-black rounded-lg"
						type="text" 
					/>
				</form>
			</div>

		</div>

  </div>
</template>

<style lang="scss" scoped>

	.navbar {
		margin-top: 49px;
		width: calc(100% - (76px * 2));
		max-width: 1920px;
	}

	.avatar {
		background-color: #FFBE40;
		width: 30px;
		height: 30px;
		font-family: PT Sans;
		font-style: normal;
		font-weight: bold;
		font-size: 16px;
		// text-align: center;
		color: #FFFFFF;
	}

	.search-bar {
		width: 190px;
		height: 30px;
		background: #F2F2F2;
		border-radius: 30px;
		border: 0px;
	}

	.user-name {
		font-family: PT Sans;
		font-weight: 700;
		font-size: 18px;
		line-height: 22px;
		color: #38547B;
	}

</style>