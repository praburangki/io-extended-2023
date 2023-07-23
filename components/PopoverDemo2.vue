<script lang="ts" setup>
import { watch } from 'vue';

watch(() => $slidev.nav.clicks, (_val) => {
  if (_val === 2) {
    const popover = document.getElementById('pop');

    setTimeout(() => {
      popover.showPopover();
    }, 100);
  }
});
</script>

<template>
  <div class="flex items-center justify-center mt-40">
    <button
      class="tokped"
    >
      Beli Langsung
    </button>

    <div
      id="pop"
      popover
    >
      Banyak hutang ga usah banyak gaya!
    </div>
  </div>
</template>

<style lang="postcss" scoped>
@import "https://unpkg.com/open-props/open-props.min.css";

  button.tokped {
    background-color: var(--NN0,#FFFFFF);
    border: 1px solid var(--GN500,#00AA5B);
    border-radius: 8px;
    color: var(--GN500,#00AA5B);
    cursor: pointer;
    display: block;
    font-family: inherit;
    font-weight: 800;
    font-size: 1rem;
    height: 40px;
    line-height: 20px;
    outline: none;
    position: relative;
    padding: 0px 16px;
    text-indent: initial;
    transition: background-color 300ms ease 0s;
    margin: 8px 0px;
  }

  [popover] {
  background: var(--gray-0);
  color: var(--gray-10);
  padding: var(--size-6);
  font-size: 2rem;
  font-weight: bold;
  overflow: visible;
}

[popover]::backdrop {
  animation: fade-in 0.25s;
  background: hsl(0 0% 0% / 0.25);
  backdrop-filter: blur(4px);
}

[popover]:popover-open {
  animation: pop 0.25s var(--ease-elastic-5);
}

@keyframes pop {
  0% {
    translate: 0 100%;
    scale: 0;
  }
}

@keyframes fade-in {
  0% {
    opacity: 0;
  }
}
</style>
