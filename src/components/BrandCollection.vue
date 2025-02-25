<script setup lang="ts">
import BrandLogo from '@/components/BrandLogo.vue'
import jollyTimeLogo from '@/assets/images/jolly-time.png'

const brands = [
  {
    imageSrc: jollyTimeLogo,
    altText: 'JollyTime Popcorn Brand Logo',
  },
  // TODO Add more brands
]
</script>

<template>
  <div class="brands">
    <BrandLogo
      v-for="brand in brands"
      :key="brand.imageSrc"
      :imageSrc="brand.imageSrc"
      :altText="brand.altText"
    />
  </div>
</template>

<style scoped>
.brands {
}
</style>
