<template>
  <a>{{ mystr }}</a>
</template>

<script setup lang="ts">
const props = defineProps({
  mystr: {
    type: String,
    required: true,
  },
});
</script>
