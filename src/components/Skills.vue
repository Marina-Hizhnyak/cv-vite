<template>
  <!--tech skills section-->
  <div class="mb-10">
    <h3 class="sidebar-title">Tech Skills</h3>
    <ul class="list-disc pl-5">
      <li v-for="skill in skills" :key="skill" class="text-orange-500 p-1">
        <span class="text-white">{{ skill }}</span>
      </li>
    </ul>
  </div>
</template>

<script setup>
import { ref } from 'vue'

const skills = ref([
  'HTML5, CSS3',
  'GIT, GitHub',
  'WebPack, Vite',
  'JavaScript',
  'PHP',
  'SQL',
  'Vue.js',
  'Laravel',
  'TailwindCSS, Bootstrap',
    'Wordpress',
  'Photoshop'
])
</script>