<script setup lang="ts">
import { ref } from 'vue'
import WebApp from '@twa-dev/sdk'

defineProps<{ msg: string }>()

const count = ref(0)

WebApp.showAlert(`Hello World!`)
</script>

<template>
  <h1>{{ msg }}</h1>

  <div class="card">
    <button type="button" @click="count++">count is {{ count }}</button>
    <p>
      Edit
      <code>components/HelloWorld.vue</code> to test HMR
    </p>
  </div>
</template>

<style scoped>

</style>
