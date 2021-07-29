<template>
	<div class="container-box w-full flex flex-col justify-center justify-items-center items-center">
		<SearchForm />
		<FilterCategory />
		<Results />
	</div>
</template>

<style lang="scss">
	.container-box {
		// min-height: 734px;
		// height: 734px;
			// position: absolute;
			margin-top: 76px;
			// min-height: 734px;
	}
</style>

<script>
import SearchForm from './SearchForm';
import FilterCategory from './FilterCategory';
import Results from './Results';

export default {
    components: {
        SearchForm,
				FilterCategory,
				Results,
    }
};

</script>
