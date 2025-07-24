<template>
  <div class="tw-w-[390px] tw-mx-auto">
    <ClientOnly>
      <NuxtClientFallback>
        <p>rendering</p>
      </NuxtClientFallback>
      <Map />
    </ClientOnly>
    <button @click="open = true">Open Modal</button>

    <teleport to="body">
      <div v-if="open" class="modal">
        <p>This is a modal window</p>
        <button @click="open = false">Close</button>
      </div>
    </teleport>
  </div>
</template>

<script setup>
import { ref } from "vue";
const open = ref(false);
</script>

<style lang="scss" scoped></style>
