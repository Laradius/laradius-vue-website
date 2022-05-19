<template>
  <div>
    <p class="fs-4">
      <i :class="iconType" :color="iconColor"></i>

      <a v-if="isLink" :href="text"> {{ text }}</a>
      <span v-else>{{ text }}</span>
    </p>
  </div>
</template>

<script setup lang="ts">
import { defineProps } from "Vue";

interface IIcon {
  iconType: string;
  iconColor: string;
  text: string;
  isLink: boolean;
}

defineProps<IIcon>();
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->

<style scoped>
span,
a {
  margin-left: 5px;
}

a {
  color: var(--primary-text) !important;
  text-decoration: none;
  border-bottom: 2px solid var(--primary);
}

a:hover {
  color: var(--primary-hover) !important;
}

div {
  vertical-align: middle;
}
</style>
