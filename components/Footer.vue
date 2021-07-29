<template>
  <div class="w-full footer-box flex justify-center">
    <div class="footer-nav divide-y divide-gray-800">
      <div class="flex flex-row justify-between pt-12">
      <!-- Footer links -->
        <div class="grid grid-flow-row grid-cols-4 grid-rows-1 gap-20">
          <!-- Customer -->
          <div class="flex flex-col">
            <div class="title-name">
              Customer
            </div>
            <ul class="mt-2.5 list-links">
              <li><a href="#">Post A Job</a></li>
              <li><a href="#">Business Directory</a></li>
              <li><a href="#">Job Cost Guides</a></li>
              <li><a href="#">Help</a></li>
            </ul>
          </div>

          <!-- Business -->
          <div class="redirect-links flex flex-col">
            <div class="title-name">
              Business
            </div>
            <ul class="mt-2.5 list-links">
              <li><a href="#">Register Business</a></li>
              <li><a href="#">Help</a></li>
            </ul>
          </div>

          <!-- About -->
          <div class="redirect-links flex flex-col">
            <div class="title-name">
              About
            </div>
            <ul class="mt-2.5 list-links">
              <li><a href="#">About us</a></li>
              <li><a href="#">Reviews</a></li>
              <li><a href="#">How it Works</a></li>
              <li><a href="#">Our Team</a></li>
              <li><a href="#">Contact Us</a></li>
            </ul>
          </div>

          <!-- Get Update -->
          <div class="redirect-links flex flex-col">
            <div class="title-name">
              Get Updated
            </div>
            <ul class="mt-2.5 list-links">
              <li><a href="#">News</a></li>
              <li><a href="#">We’re Hiring</a></li>
            </ul>
          </div>
        </div>

        <!-- Download Section -->
        <div class="flex flex-col ml-80">
            <div class="title-name">
              Download our apps
            </div>
            <img class="download-apps mt-2.5" :src="require('~/assets/images/download-apps.png')" />
          </div>
      </div>

      <!-- Footer rights -->
      <div class="w-full mt-11 flex flex-row items-center justify-between">
        <div class="flex flex-row mt-3.5 items-end">
          <p class="logo-name">Logo</p>
          <p class="ml-5 alrights-reserve">© 2021 The Local Pro. All Rights Reserved.</p>
        </div>

        <ul class="mt-2.5 list-links flex flex-row gap-8">
          <li><a href="#">Terms of use</a></li>
          <li><a href="#">Privacy Policy</a></li>
        </ul>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
  .footer-box {
    margin-top: 150px;
    min-height: 340px;
    left: 0px;
    background: #F1F8FF;
    mix-blend-mode: normal;
  }

  .footer-nav {
    // width: calc(100% - (397px * 2));
    // width: calc(100% - (397px * 2));
		max-width: 1920px;
    // background-color: red;
  }

  .title-name {
    // font-size: 18px;
    font-style: normal;
    font-weight: bold;
    font-size: calc((1920vw / 18) * 100%);
    line-height: 22px;
    color: #38547B;
  }

  .list-links a {
    font-style: normal;
    font-weight: normal;
    // font-size: 13px;
    font-size: calc((1920vw / 18) * 100%);
    line-height: 16px;
    color: #38547B;
  }

  .list-links + a{
    margin-bottom: 10px;
  }

  .download-apps {
    width: calc((1920vw / 159vw) * 100%);
    height: auto;
  }

  .logo-name {
    font-style: normal;
    font-weight: bold;
    font-size: 25px;
    line-height: 30px;

    color: #000000;
  }

  .alrights-reserve {
    font-style: normal;
    font-weight: normal;
    font-size: 13px;
    line-height: 16px;
    color: #38547B;
  }
</style>