<script setup lang="ts">
const props = defineProps({
  image: {
    type: String,
    required: true
  },
  alt: {
    type: String,
    required: true
  }
})
</script>

<template>
  <div class="card">
    <img :src="props.image" :alt="props.alt" />
    <div class="card-content">
      <slot />
    </div>
  </div>
</template>

<style scoped>
.card {
  width: 20rem;
  padding: 1rem;
  box-sizing: border-box;
  border-radius: 1rem;
  background-color: hsl(0, 0%, 100%);
  box-shadow: 0 1.5rem 1.5rem hsl(220, 15%, 55%, 10%);
}
.card-content {
  text-align: center;
  padding: 0.25rem 1rem 0.5rem 1rem;
}
img {
  width: 100%;
  border-radius: 0.5rem;
}
</style>
