<script setup lang="ts">
useHead({
  title: "login",
});

const emailRef = ref("");
const passwordRef = ref("");
const nameRef = ref("");
</script>

<template>
  <div class="flex items-center justify-center min-h-screen w-full">
    <div class="rounded bg-sidebar w-1/2 p-5">
      <h1 class="text-2xl font-bold text-center mb-5">Login</h1>
      <form class="text-white">
        <a-space direction="vertical" style="width: 100%">
          <a-input
            v-model:value="nameRef"
            placeholder="name"
            type="text"
            class="mb-3 bg-transparent text-white placeholder:text-slate-400"
          />
          <a-input
            v-model:value="emailRef"
            placeholder="email"
            type="email"
            class="mb-3 bg-transparent text-white placeholder:text-slate-400"
          />
          <a-input
            type="password"
            v-model:value="passwordRef"
            placeholder="password"
            class="mb-3 bg-transparent text-white placeholder:text-slate-400"
          >
          </a-input>
          <div class="flex items-center justify-center gap-5 w-full">
            <a-button class="text-white w-1/2">Login</a-button>
            <a-button class="text-white w-1/2">Register</a-button>
          </div>
        </a-space>
      </form>
    </div>
  </div>
</template>

<style scoped></style>
