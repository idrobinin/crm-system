<script lang="ts" setup>
const config = useRuntimeConfig();
const COLLECTION_COMMENTS = config.APPWRITE_DEFAULT_ENDPOINT;
console.log(COLLECTION_COMMENTS);
</script>

<template>
  <section class="grid" style="min-height: 100vh">
    <LayoutSidebar />

    <div>
      <slot />
    </div>
  </section>
</template>

<style scoped>
.grid {
  display: grid;
  grid-template-columns: 1fr 6fr;
}
</style>
