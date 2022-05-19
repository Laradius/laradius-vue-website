<template>
  <div>
    <Jumbotron
      title="Quick introduction"
      text=" Hello, my name is Elliot. My main interests include programming and electronics. 
      I mostly use C# (WPF, Razor Pages, .NET Core Rest API) and TypeScript with Vue.js to develop various applications. 
      In my free time, I like to listen to music, learn about psychology and develop other smaller intrests."
    >
      <button class="button-primary btn btn-lg" type="button">
        Learn more about me
      </button>
    </Jumbotron>
  </div>
</template>

<script setup lang="ts">
import Jumbotron from "@/components/Jumbotron.vue";
</script>
