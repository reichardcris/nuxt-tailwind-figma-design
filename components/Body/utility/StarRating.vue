<template>
  <div class="p-none flex flex-row">
    <img v-for="stars in 5" :key="stars" :src="require('~/assets/images/icons/star.svg')" alt="star">
  </div>
</template>

<style lang="scss" scoped>
 img {
  width: 20px;
  height: 20px;
 }
</style>