<template>
  <div>
    <h1 class="title">Test</h1>
    <NuxtLink to="/">home</NuxtLink>
  </div>
</template>

<script setup>
import gsap from 'gsap';

onMounted(() => {
  const tlHero = gsap.timeline();
  tlHero.addLabel('start');
  tlHero.from('.title', { y: 60, opacity: 0, duration: 1.2 }, 'start');
});
</script>
