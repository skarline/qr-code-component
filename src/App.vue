<script setup lang="ts">
import MyCard from "./components/MyCard.vue"
</script>

<template>
  <MyCard image="./image-qr-code.png" alt="frontendmentor.io">
    <h1>Improve your front-end skills by building projects</h1>
    <p>
      Scan the QR code to visit Frontend Mentor and take your coding skills to
      the next level
    </p>
  </MyCard>
</template>

<style>
body {
  font-family: "Outfit", sans-serif;
  display: grid;
  place-items: center;
  height: 100vh;
  background-color: hsl(212, 45%, 89%);
}
h1 {
  color: hsl(218, 44%, 22%);
  font-size: 22px;
}
p {
  color: hsl(220, 15%, 55%);
  font-size: 15px;
}
</style>
