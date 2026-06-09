<script setup>
import homeData from '../content/home.json'
</script>

<template>
  <section class="hero">
    <h1>{{ homeData.title }}</h1>

    <p>{{ homeData.subtitle }}</p>

    <img :src="homeData.heroImage" />

    <a :href="'tel:' + homeData.phone">
      {{ homeData.phone }}
    </a>
  </section>
</template>
