<template>
  <div class="absolute inset-0 z-1">
    <div class="bg-white w-full h-10 top-0 left-0 right-0 z-20 absolute" />

    <div class="pt-24 pb-10 px-8 flex flex-col h-full w-1/4">
      <BrowserSupport
        v-click
        :browsers="[
          {
            name: 'chrome',
            supported: 'yes',
            version: 111,
          },
          {
            name: 'firefox',
            supported: 'no',
            version: '',
          },
          {
            name: 'edge',
            supported: 'yes',
            version: 111,
          },
          {
            name: 'safari',
            supported: 'no',
            version: '',
          },
        ]"
      />

      <h3
        v-click
        class="font-semibold mt-20"
      >
        Mobile dev?
      </h3>
    </div>

    <video
      src="https://res.cloudinary.com/ddxwdqwkr/video/upload/v1678492898/patterns.dev/astro-movies-2023.mp4"
      autoplay
      playsinline
      muted
      loop
      class="h-full absolute top-5 -right-4"
    >
      <source
        src="https://res.cloudinary.com/ddxwdqwkr/video/upload/v1678492898/patterns.dev/astro-movies-2023.mp4"
        type="video/mp4"
      >
    </video>
  </div>
</template>

