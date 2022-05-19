<template>
  <div class="py-3 text-center container-fluid">
    <div class="text-sm-start container">
      <div class="row">
        <div class="col-sm">
          <div
            class="h-100 flex-column align-items-start justify-content-center d-sm-flex"
          >
            <h3 class="mb-sm-5">Contact Info:</h3>
            <ContactInfo
              iconType="fa-2xl fa-solid fa-envelope"
              iconColor="var(--secondary)"
              text="elliotwhite@gmail.com"
              :isLink="false"
            />
            <ContactInfo
              iconType="fa-2xl fa-brands fa-github"
              iconColor="var(--secondary)"
              text="https://github.com/Laradius"
              :isLink="true"
            />
          </div>
        </div>
        <ContactForm class="col-sm-4" />
      </div>
    </div>
    <p class="align-self-end fs-5 pb-1 py-3">{{ copyright }}</p>
  </div>
</template>

<script setup lang="ts">
import { defineProps } from "Vue";
import ContactForm from "./ContactForm.vue";
import ContactInfo from "./ContactInfo.vue";

interface IFooter {
  copyright: string;
}

defineProps<IFooter>();
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.container-fluid {
  background-color: var(--paper-background);
}

p {
  margin-bottom: 0;
}
</style>
