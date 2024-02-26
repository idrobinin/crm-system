<script lang="ts" setup></script>

<template>
  <aside class="px-5 py-8 bg-sidebar h-full relative w-full">
    <button
      type="button"
      class="absolute top-2 right-3 text-white hover:text-violet transition-colors"
    >
      <Icon name="line-md:logout" size="22px" />
    </button>
    <NuxtLink to="/" class="mb-10 mt-5 block">
      <NuxtImg src="/logo.svg" alt="" width="100px" class="mx-auto" />
    </NuxtLink>
    <div>
      <LayoutMenu />
    </div>
  </aside>
</template>
