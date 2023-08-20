<script setup>
defineProps(["message"]);
defineEmits(["messageEmitted"]);
</script>

<template>
  <div class="">
    <h3 class="text-2xl pb-3 font-semibold">Child Component</h3>
    <p class="mt-2 font-bold">Received Message : {{ message }}</p>
    <button
      @click="$emit('messageEmitted', 'This is a Custom message from Child!')"
      class="my-4 px-5 py-3 font-bold bg-gradient-to-r from-indigo-500 to-pink-500 hover:from-pink-600 hover:to-indigo-600 text-white rounded"
    >
      Emit Message
    </button>
  </div>
</template>

<style scoped></style>
