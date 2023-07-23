---
theme: ./theme
layout: intro
---



---
src: ./io-connect.md
---

---
src: ./view-transition-api.md
---

---
src: ./devtools.md
---

---
layout: image-only
image: https://media-cms.onesignal.com/cms/_800xAUTO_crop_center-center_none/web-push-trust-the-market-leader-4.jpg
imgClasses: h-[100%]
---

# Web Push Notifications

<BrowserSupport
  v-click
  :browsers="[
    {
      name: 'chrome',
      supported: 'yes',
      version: 42,
    },
    {
      name: 'firefox',
      supported: 'yes',
      version: 44,
    },
    {
      name: 'edge',
      supported: 'yes',
      version: 17,
    },
    {
      name: 'safari',
      supported: 'yes',
      version: 16,
    },
  ]"
/>

---
transition: slide-up
---

# Popover

<div class="flex items-center justify-around mt-10">
  <PopoverDemo1 />

  <v-clicks>

  - Top Layer Support
  - Light-dismiss
  - Native Accessibility
  - No Javascript Needed

  </v-clicks>
</div>


---
transition: slide-up
---

# Popover

<style>
  pre {
    padding: 16px 24px;
  }
</style>


<BrowserSupport
  v-click
  :browsers="[
    {
      name: 'chrome',
      supported: 'yes',
      version: 114,
    },
    {
      name: 'firefox',
      supported: 'no',
      version: '',
    },
    {
      name: 'edge',
      supported: 'yes',
      version: 114,
    },
    {
      name: 'safari',
      supported: 'no',
      version: '',
    },
  ]"
/>

<div class="flex items-center justify-around mt-5">
  <PopoverDemo1 />

  ```html
  <div id="event-popup" popover>
    <!-- 
      Popover content
      (i.e new event form)
      goes in here
      -->
  </div>

  <button popovertarget="event-popup">
    Create new Event
  </button
  ```
</div>

---
transition: slide-up

clicks: 2
---

# Popover

<PopoverDemo2 />

---
transition: slide-up

layout: image-only
image: /popover-demo-2.png
imgClasses: h-[100%]
---

# Popover (Anchor Positioning)

---
layout: image-only
image: https://web-dev.imgix.net/image/kheDArv5csY6rvQUJDbWRscckLr1/Gv27TPZQF9EPSZIDmpHZ.png?auto=format&w=1600
---

# Baseline

---
src: ./frameworks.md
---

---
src: './privacy.md'
---

---
layout: thanks
---


---
clicks: 12
---

<KuisMaksa />

