<script setup lang="ts">
import { MENU_DATA } from "~/components/layout/menu.data";
</script>

<template>
  <div>
    <NuxtLink
      v-for="item in MENU_DATA"
      :key="item.url"
      :to="item.url"
      class="flex items-center rounded-lg py-1 px-3 w-full mb-2 transition-all hover:bg-gray-700 hover:shadow"
    >
      <Icon :name="item.icon" />
      <span class="ml-4">{{ item.name }}</span>
    </NuxtLink>
  </div>
</template>
