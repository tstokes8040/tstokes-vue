<script setup lang="ts">
interface BrandLogoProps {
  imageSrc: string
  altText: string
}

defineProps<BrandLogoProps>()
</script>

<template>
  <div class="brand-item">
    <img :src="imageSrc" :alt="altText" />
  </div>
</template>

<style scoped>
.brand-item {
}
</style>
