<template>
  <div class="w-full flex flex-col justify-center items-center justify-contents-center" style="margin-top: 105px;">
    <div class="result-box w-full pt-5" v-for="results in 5" :key="results">
      <!-- Result Heading Details -->
      <div class="result-heading-section flex flex-row justify-between">
        <div class="result-details grid grid-flow-col">
          <!-- Logo Avatar -->
          <img :src="require('~/assets/images/company-avatar.png')" />
          <!-- Company Name -->
          <div class="result-company-name">
            <p>Imaginea</p>
            <span class="mt-1.5">Manchester</span>
						<!-- Rating Review -->
						<div class="m-t1 flex flex-row justify-center items-center justify-contents-center">
							<StarRating />
							<p class="review">100 reviews</p>
						</div>
          </div>
        </div>
        <div class="result-code-name mr-7">
          ABN 62 502 909 410
        </div>
      </div>
      <!-- Result Description -->
      <div class="result-description">
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore
        magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
        consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
        Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
      </div>

			<!-- Requet Button -->
			<div class="w-full flex justify-center mt-14">
				<button class="request-button">
					Request Quote
				</button>
			</div>
			
    </div>

		<!-- See more button -->
		<div class="w-full flex flex-row justify-center items-center justify-contents-center">
			<button class="see-more-button">
				See more
			</button>
		</div>
  </div>
</template>

<script>
import StarRating from './utility/StarRating';

export default {
  components: {
		StarRating,
	}
}
</script>

<style lang="scss" scoped>
  .result-box {
    max-width: 1016px;
    height: 477px;
    // margin-top: 105px;
    background: #FFFFFF;
    box-shadow: 0px 35px 50px rgba(0, 0, 0, 0.05);
    border-radius: 20px;
    // border: 1px solid #000;
		+ div {
			margin-top: 100px;
		}
  }

  .result-details {
    margin-left: 50px;
    img {
      width: 61px;
      height: 67px;
    }
  }
	

  .result-company-name {
    margin-left: 50px;
    font-style: normal;
    font-weight: bold;
    font-size: 20px;
    line-height: 24px;
    color: #38547B;

    span {
      font-style: normal;
      font-weight: normal;
      font-size: 18px;
      line-height: 22px;
    }
  }

  .result-code-name {
    font-style: normal;
    font-weight: bold;
    font-size: 18px;
    line-height: 22px;
    color: #D6D6D6;
  }

  .result-description {
    margin-top: 60px;
    margin-left: 160px;
    margin-right: 88px;
		font-family: PT Sans;
	  font-style: normal;
		font-weight: normal;
		font-size: 16px;
    line-height: 35px;
    color: #38547B !important;
  }

	.review {
		font-family: PT Sans;
		font-weight: 700;
		margin-left: 15px;
		font-size: 16px;
		// line-height: 19px;
		text-decoration-line: underline;
		color: #38547B;
		cursor: pointer;
	}

	.request-button {
		font-family: PT Sans;
		font-weight: 700;
		color:  #fff;
		width: 200px;
		height: 52px;
		left: 892px;
		background: #38547B;
		border-radius: 5px;
	}

	.see-more-button {
		width: 100%;
		max-width: 145px;
		height: 55px;
		border: 1px solid #38547B;
		box-sizing: border-box;
		border-radius: 5px;
		font-style: normal;
		font-weight: bold;
		font-size: 22px;
		line-height: 27px;
		color: #38547B;
	}
</style>
