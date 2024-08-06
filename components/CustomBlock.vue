<template>
  <div
    class="custom-block"
    v-bind="{
      class: color,
    }"
  >
    <slot />
  </div>
</template>

<script setup lang="ts">
withDefaults(
  defineProps<{
    color: 'red' | 'blue';
  }>(),
  {
    color: 'red',
  }
);
</script>
