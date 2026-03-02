<script setup>
import { RouterLink } from "vue-router";
</script>

<template>
  <div class="content-wrap">
    <h1
      class="name-title"
      style="
        font-size: 36px;
        margin-bottom: 2px;
        letter-spacing: -2px;
        margin-top: 40px;
      "
    >
      Coming Soon
    </h1>

    <p class="location-text" style="font-size: 18px; margin-bottom: 10px">
      This game is currently under development
    </p>

    <RouterLink
      to="/arcade"
      class="repo-link"
      style="margin-top: 20px; font-size: 16px; display: inline-block"
    >
      ← Back to arcade
    </RouterLink>
  </div>
</template>
