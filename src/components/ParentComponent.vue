<script setup>
import { ref } from "vue";
import ChildComponent from "./ChildComponent.vue";

const message = ref("Hello I'm from Parent Component!");
const emittedMessage = ref("");

const handleMessageEmitted = (message) => {
  emittedMessage.value = message;
};
</script>

<template>
  <div
    class="border-double border-4 border-indigo-300 rounded p-10 shadow-2xl shadow-blue-500/20"
  >
    <ChildComponent :message="message" @messageEmitted="handleMessageEmitted" />
    <p class="font-bold">
      Emitted Message: <span class="italic">{{ emittedMessage }}</span>
    </p>
  </div>
</template>

<style scoped></style>
