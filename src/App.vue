<script setup>
import ParentComponent from "./components/ParentComponent.vue";
</script>

<template>
  <div
    class="bg-gradient-to-r from-pink-100 via-indigo-100 to-pink-100 h-screen flex flex-col justify-center items-center text-center"
  >
    <h2 class="text-4xl mb-5 font-semibold">Parent Component</h2>

    <ParentComponent />
  </div>
</template>

<style scoped></style>
