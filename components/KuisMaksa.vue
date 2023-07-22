<script lang="ts" setup>
</script>

<template>
  <h1 class="font-bold text-center">
    Kuis Maksa
  </h1>

  <div class="h-20">
    <div
      v-click="1"
      class="items-center px-20"
      :class="{
        hidden: $slidev.nav.clicks > 3,
        flex: $slidev.nav.clicks <= 3,
      }"
    >
      <img
        src="https://upload.wikimedia.org/wikipedia/commons/thumb/0/04/ChatGPT_logo.svg/440px-ChatGPT_logo.svg.png"
        alt=""
        class="w-20 h-20"
      >
      <span class="ml-8">
        Chat GPT adalah sistem kecerdasan buatan AI yang berfungsi untuk melakukan interaksi dalam percakapan berbasis teks.
      </span>
    </div>
    <div
      class="justify-center items-center gap-4 font-semibold h-full"
      :class="{
        hidden: $slidev.nav.clicks < 4,
        flex: $slidev.nav.clicks >= 4,
      }"
    >
      <div
        v-click="4"
        class="rounded-5 border-2 border-black text-center px-4 bg-black/10 tracking-wide"
      >
        Ganteng
      </div>
      <div
        v-click="5"
        class="rounded-5 border-2 border-black text-center px-4 bg-black/10 tracking-wide"
      >
        Sing Main-Main
      </div>
      <div
        v-click="6"
        class="rounded-5 border-2 border-black text-center px-4 bg-black/10 tracking-wide"
      >
        2024
      </div>
      <div
        v-click="7"
        class="rounded-5 border-2 border-black text-center px-4 bg-black/10 tracking-wide"
      >
        Bestie
      </div>
    </div>
  </div>

  <h2
    v-click="2"
    class="mt-4 text-center"
  >
    Apa kepanjangan dari <strong>GPT</strong> ?
  </h2>

  <div
    v-click="3"
    class="uppercase mt-4 text-[50px] flex flex-col items-center"
  >
    <div class="flex">
      <div
        class="kuis-word"
        :class="{
          ngenah: $slidev.nav.clicks > 9,
        }"
      >
        <div><span>g</span></div>
        <div><span>a</span></div>
        <div><span>n</span></div>
        <div><span>j</span></div>
        <div><span>a</span></div>
        <div><span>r</span></div>
      </div>

      <div
        class="ml-8 kuis-word"
        :class="{
          ngenah: $slidev.nav.clicks > 10,
        }"
      >
        <div><span>p</span></div>
        <div><span>r</span></div>
        <div><span>a</span></div>
        <div><span>b</span></div>
        <div><span>o</span></div>
        <div><span>w</span></div>
        <div><span>o</span></div>
      </div>
    </div>

    <div
      class="kuis-word mt-6"
      :class="{
        ngenah: $slidev.nav.clicks > 11,
      }"
    >
      <div><span>t</span></div>
      <div>
        <span>
          e
        </span>
      </div>
      <div>
        <span
          :class="{
            ngenah: $slidev.nav.clicks > 7,
          }"
        >
          m
        </span>
      </div>
      <div>
        <span>
          e
        </span>
      </div>
      <div>
        <span
          :class="{
            ngenah: $slidev.nav.clicks > 8,
          }"
        >
          n
        </span>
      </div>
      <div>
        <span>
          a
        </span>
      </div>
      <div>
        <span
          :class="{
            ngenah: $slidev.nav.clicks > 8,
          }"
        >
          n
        </span>
      </div>
    </div>
  </div>
</template>

<style lang="postcss" scoped>
  .kuis-word {
    display: flex;

    > div {
      width: 50px;
      display: flex;
      justify-content: center;
      margin-left: 12px;
      border-bottom: 2px solid black;

      > span {
        filter: blur(15px);

        &.ngenah {
          filter: blur(0);
        }
      }
    }

    &.ngenah {
      > div {
        > span {
          filter: blur(0);
        }
      }
    }
  }
</style>

