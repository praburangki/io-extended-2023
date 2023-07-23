<script lang="ts" setup>

</script>

<template>
  <div class="slidev-layout bg-[#29AB49] relative pa-6">
    <div class="shape yellow-circle" />
    <div class="shape white-circle" />
    <div class="shape blue-circle" />
    <div class="shape red-box" />
    <div class="line" />

    <div class="h-full relative bg-white rounded-4 border-black border-4 pa-8 overflow-hidden flex flex-col">
      <slot />
    </div>
  </div>
</template>

<style lang="postcss" scoped>
  .shape {
    position: absolute;
    border: 3px solid black;
  }

  .yellow-circle {
    border-radius: 9999px;
    width: 220px;
    height: 220px;
    background: #FFBB00;
    top: 81px;
    left: -39px;
  }

  .white-circle {
    border-radius: 9999px;
    width: 240px;
    height: 240px;
    background: #E8E9EC;
    top: -30px;
    left: 241px;
  }

  .blue-circle {
    background: #3C8AFF;
    bottom: -40px;
    left: 212px;
    width: 175px;
    height: 175px;
    border-radius: 9999px;
  }

  .red-box {
    transform: rotate(70deg);
    background: #FF4F3F;
    bottom: -16px;
    left: -2px;
    width: 200px;
    height: 190px;
    border-radius: 24px;
  }

  .line {
    width: 300px;
    transform: rotate(-23deg);
    top: 26px;
    left: 30px;
    height: 3px;
    background: black;
    border: none;
    position: absolute;;
  }
</style>
