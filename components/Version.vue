<script setup lang="ts">
import 'vue';
import packageJson from '../package.json';
</script>

<template>
  <span>Version {{ packageJson.version }}</span>
</template>
