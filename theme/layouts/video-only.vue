<script lang="ts" setup>
defineProps({
  video: String,
  videoClasses: String,
});
</script>

<template>
  <BaseLayout>
    <div class="flex flex-col h-full">
      <slot />

      <div class="flex-1 relative">
        <video
          playsinline
          muted
          loop
          autoplay
          :class="videoClasses"
        >
          <source
            src="https://storage.googleapis.com/web-dev-uploads/video/NJdAV9UgKuN8AhoaPBquL7giZQo1/2KQ2gCmcR6mGKO29wCJH.mp4"
            type="video/mp4"
          >
        </video>
      </div>
    </div>
  </BaseLayout>
</template>
