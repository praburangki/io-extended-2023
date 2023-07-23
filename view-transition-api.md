---
transition: slide-up
---

# View Transition API

<VTADemo1 />

---
transition: slide-up
---

# View Transition API

<VTADemo2 />

<style>
.slidev-code-wrapper {
  font-size: 14px;
}
</style>

<v-click>
```css
  ::view-transition-old(root), ::view-transition-new(root) {
    animation: none;
    mix-blend-mode: normal;
  }
  ::view-transition-old(root) {
    z-index: 9999;
  }
  ::view-transition-new(root) {
    z-index: 1;
  }
  .dark::view-transition-old(root) {
    z-index: 1;
  }
  .dark::view-transition-new(root) {
    z-index: 9999;
  }
```
</v-click>

---
transition: slide-up
---

# View Transition API

<VTADemo2 />

<style>
.slidev-code-wrapper {
  font-size: 14px;
}
</style>

```ts
  if (!document.startViewTransition) {
    toggleColorMode();
    return;
  }

  const viewTransition = document.startViewTransition(() => {
    toggleColorMode();
  });

  viewTransition.ready.then(() => {
    // Animate the transition
    // Habis itu bebas mau ngapain aja
  });
```

<div class="mt-8 font-semibold">
github.com/praburangki/praburangki.dev
</div>

---
transition: slide-up
---

# View Transition API

<VTADemo3 />
