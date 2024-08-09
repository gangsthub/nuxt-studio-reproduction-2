<template>
  <div class="custom-block">
    <h3>{{ title }}</h3>
    <slot />
    <div class="image-wrapper" v-if="$slots.image">
      <slot name="image" />
    </div>
  </div>
</template>

<script setup lang="ts">
defineProps<{
  title: string;
}>();

defineSlots<{
  default: any;
  image: any;
}>();
</script>
