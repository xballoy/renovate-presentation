<script setup lang="ts">
import 'vue';
import { format } from 'date-fns';

const props = defineProps({
  dateFormat: {
    default: 'PP',
  },
});

</script>

<template>
  <span>{{ format(new Date(), props.dateFormat) }}</span>
</template>
