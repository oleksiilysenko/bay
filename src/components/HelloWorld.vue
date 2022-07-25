<template>
  <h1>{{ msg }}</h1>

  <p>
    <a href="https://e.mail.ru" target="_blank">
      Mail Box
    </a>
    |||||
    <a href="https://google.com/" target="_blank">Google Search</a>
  </p>

  <button type="button" @click="state.count++">count is: {{ state.count }}</button>
  <p>
     <h1>This is a temmplate for pages<h1>
    
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
