<script setup lang="ts">
import { ref } from 'vue'

defineProps({
  title: String,
    description: String,
})

const count = ref<Number>(0)
</script>

<template>
  <h1>{{ title }}</h1>
    <p>{{description}}</p>
  <div class="card">
    <button type="button" @click="count++">count is {{ count }}</button>
  </div>
</template>
