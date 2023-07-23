<script lang="ts" setup>
defineProps({
  image: String,
  imgClasses: String,
});
</script>

<template>
  <BaseLayout>
    <div class="flex flex-col h-full">
      <slot />

      <div class="flex-1 relative">
        <img
          :src="image"
          class="absolute inset-0 mx-auto max-w-full"
          :class="imgClasses"
        >
      </div>
    </div>
  </BaseLayout>
</template>
