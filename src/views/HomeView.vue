<script setup>
import { ref } from 'vue'

const title = ref('Добро пожаловать на наш веб-ресурс')
const features = ref([
  'Современный интерфейс',
  'Быстрая загрузка',
  'Адаптивная верстка'
])
</script>

<template>
  <main class="home">
    <h1>{{ title }}</h1>
    <ul>
      <li v-for="feature in features" :key="feature">{{ feature }}</li>
    </ul>
  </main>
</template>

<style scoped>
.home {
  max-width: 900px;
  margin: 0 auto;
  padding: 2rem;
}
</style> 