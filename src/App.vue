<template>
  <Navbar />
  <router-view />
  <Footer copyright="&copy; White Software 2022"></Footer>
</template>

<script setup lang="ts">
import Navbar from "./components/Navbar.vue";
import Footer from "./components/Footer.vue";
</script>

<style>
:root {
  --site-background: #303030;
  --paper-background: #424242;
  --primary: #8c3bc4;
  --primary-text: #fff;
  --primary-hover: rgba(255, 255, 255, 0.9);
  --primary-secondary-text: rgba(255, 255, 255, 0.7);
  --secondary: #73c43b;
  --secondary-text: rgba(0, 0, 0, 0.87);
  --secondary-text-hover: rgba(0, 0, 0, 0.7);
}

body {
  background-color: var(--site-background) !important;
  color: var(--primary-text) !important;
}

.button-primary {
  transition: unset !important;
  background-color: var(--primary) !important;
  color: var(--primary-text) !important;
}

.button-primary:hover {
  color: var(--primary-hover) !important;
}

.button-secondary {
  transition: unset;
  background-color: var(--secondary) !important;
  color: var(--secondary-text) !important;
}

.button-secondary:hover {
  color: var(--secondary-text-hover) !important;
}
</style>
