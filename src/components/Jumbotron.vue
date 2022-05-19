<template>
  <div class="text-center container-fluid py-5">
    <h1>{{ title }}</h1>
    <p class="fs-4">
      {{ text }}
    </p>
    <slot></slot>
  </div>
</template>

<script setup lang="ts">
import { defineProps } from "Vue";

interface IJumbotron {
  title: string;
  text: string;
}

defineProps<IJumbotron>();
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.container-fluid {
  color: var(--primary-text);
  background-image: url("../assets/sky.png");
  background-size: cover;
  background-repeat: no-repeat;
  background-position: 50% 50%;
}

p {
  white-space: pre-wrap;
}

button {
  transition: unset;
  background-color: var(--primary);
  color: var(--primary-text);
}

button:hover {
  color: var(--primary-hover);
}
</style>
