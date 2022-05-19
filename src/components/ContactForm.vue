<template>
  <div class="text-center messageForm py-3">
    <div class="mb-3">
      <label for="emailAddress" class="form-label">Email address</label>
      <input
        type="email"
        class="form-control"
        id="emailAddress"
        placeholder="youraddress@example.com"
      />
    </div>
    <div class="mb-3">
      <label for="message" class="form-label">Message</label>
      <textarea class="form-control" id="message" rows="2"></textarea>
    </div>

    <div class="mb-3">
      <button class="button-secondary btn btn-lg" type="button">Send</button>
    </div>
  </div>
</template>

<script setup lang="ts">
import { defineProps } from "Vue";

// defineProps<IJumbotron>();
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.messageForm {
  background-color: var(--site-background);
}
</style>
