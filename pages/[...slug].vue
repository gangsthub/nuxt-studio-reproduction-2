<template>
  <main>
    <ContentDoc v-slot="{ doc }">
      <ContentRenderer :value="doc" :components="{ CustomBlock }" />
    </ContentDoc>
  </main>
</template>

<script setup lang="ts">
import { CustomBlock } from '#components';
</script>
