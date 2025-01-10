<template>
  <svg viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg" :class="svgClass">
    <path stroke="none" d="M0 0h24v24H0z" fill="none" />
    <path d="M4 6l16 0" />
    <path d="M4 12l16 0" />
    <path d="M4 18l16 0" />
  </svg>
</template>

<script setup>
import { defineProps } from "vue";

const props = defineProps({
  svgClass: {
    type: String,
    default: "",
  },
});
</script>
