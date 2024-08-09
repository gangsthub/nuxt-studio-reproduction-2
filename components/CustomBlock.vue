<template>
  <div class="custom-block">
    <h1>{{ title }}</h1>
    <slot />
  </div>
</template>

<script setup lang="ts">
defineProps<{
  title: string;
}>();
</script>
