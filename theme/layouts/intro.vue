<template>
  <BaseLayout>
    <div class="flex items-center justify-between h-full pl-4">
      <SlideTitle />

      <div class="flex flex-col items-center pr-8 transition">
        <img
          class="w-60 h-60 rounded-full border-black border-3"
          src="/avatar-cang.jpg"
          alt=""
        >

        <h2 class="font-bold mt-4">
          Prabu Rangki
        </h2>

        <h4 class="font-bold text-black/70 mt-2">
          Frontend Lead @ Kintell
        </h4>

        <h4
          v-click
          class="font-bold text-[#FFBB00] mt-2"
        >
          Si Paling Startup
        </h4>

        <h4
          class="font-bold text-[#29AB49] mt-2 gde"
        >
          <span
            v-click
          >
            Google Developer Expert
          </span>
          <span
            v-click
          >
            Penjilat
          </span>
        </h4>
      </div>
    </div>
  </BaseLayout>
</template>
