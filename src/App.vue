<script setup></script>

<template>
  <div class="zoop">
    <div style="display: flex">
      <p
        v-motion
        :initial="{ opacity: 0, x: -500, y: -500, rotate: -90 }"
        :enter="{ opacity: 1, x: 0, y: 0, rotate: 0 }"
        :delay="800"
      >
        👉
      </p>
      <p
        v-motion
        :initial="{ opacity: 0, y: -500 }"
        :enter="{ opacity: 1, y: 0 }"
        :delay="400"
      >
        😎
      </p>
      <p
        v-motion
        :initial="{ opacity: 0, x: -500, y: -500, rotate: -90 }"
        :enter="{ opacity: 1, x: 0, y: 0, rotate: 0 }"
        :delay="900"
      >
        👉
      </p>
    </div>
    <p
      v-motion
      :initial="{ opacity: 0, x: -500 }"
      :enter="{ opacity: 1, x: 0 }"
      :delay="1300"
    >
      zoop
    </p>
  </div>
</template>

<style>
@import url("https://fonts.googleapis.com/css2?family=Permanent+Marker&display=swap");

html,
body {
  padding: 0;
  margin: 0;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100%;
  font-family: "Permanent Marker", cursive;
}

/* prefers dark */
@media (prefers-color-scheme: dark) {
  html,
  body {
    background-color: #333;
    color: #fff;
  }
}

.zoop {
  font-size: 15vw;
  text-align: center;
}

p {
  margin: 0;
  padding: 0;
}
</style>
