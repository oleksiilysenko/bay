<template>
  <h1>{{ msg }}</h1>

  <p>
    <a href="https://google.com" target="_blank">Search</a>
    |
    <a href="https://mail.ru" target="_blank">Mail</a>
  </p>

  <button type="button" @click="state.count++">count is: {{ state.count }}</button>
  <p>
    Edit
    <code>components/HelloWorld.vue</code> to test hot module replacement.
  </p>
</template>

<script setup>
import { defineProps, reactive } from 'vue'

defineProps({
  msg: String
})

const state = reactive({ count: 0 })
</script>

<style scoped>
a {
  color: #42b983;
}
</style>
