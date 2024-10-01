
<template>
  <div class="mb-10">
    <h3 class="text-2xl font-bold text-gray-800 mb-4">Projects</h3>
    <ul class="space-y-4">
      <li v-for="(project, index) in projects" :key="index" class="bg-white rounded-lg shadow-md overflow-hidden hover:shadow-lg transition-shadow duration-300">
        <a :href="project.url" target="_blank" rel="noopener noreferrer" class="block p-4">
          <div class="flex justify-between items-center">
            <span class="text-lg font-semibold text-orange-600 hover:text-orange-800 transition-colors duration-300">{{ project.name }}</span>
            <span class="text-sm text-gray-500">[ {{ project.technologies.join(', ') }} ]</span>
          </div>
          <p class="text-gray-600 mt-2">{{ project.description }}</p>
        </a>
      </li>
    </ul>
  </div>
</template>

<script setup>

     const projects = [
        {
          name: 'CSS Exam Project',
          url: 'https://marina-hizhnyak.github.io/examen-css/',
          technologies: ['HTML5', 'CSS3'],
          description: 'A showcase of advanced CSS techniques and responsive design.'
        },
        {
          name: 'Web Shop B-Shop',
          url: 'https://webshopbshop.vercel.app/',
          technologies: ['JavaScript', 'Vite'],
          description: 'An e-commerce platform built with modern JavaScript and Vite for fast performance.'
        },
        {
          name: 'Product Catalogue',
          url: 'http://catalogue.maryk.be/product/index',
          technologies: ['PHP'],
          description: 'A dynamic product catalogue system developed with PHP.'
        }
      ]

</script>
