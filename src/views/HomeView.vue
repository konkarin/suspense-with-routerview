<script setup lang="ts">
import { ref } from 'vue'

const message = ref('')

message.value = await new Promise((resolve) => {
  setTimeout(() => {
    resolve('home')
  }, 1000)
})
</script>

<template>
  <div>{{ message }}</div>
</template>
