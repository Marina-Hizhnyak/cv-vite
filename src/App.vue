<script setup>
import Photo from './components/Photo.vue';
import Contacts from './components/Contacts.vue';
import Skills from './components/Skills.vue';
import Hobbies from './components/Hobbies.vue';
import Languages from './components/Languages.vue';
import About from './components/About.vue';
import Projets from './components/Projets.vue';
import Experience from './components/Experience.vue';
import Education from './components/Education.vue';
</script>

<template>
  <div class="max-w-screen-xl mx-auto p-4 sm:p-6 lg:p-8">
    <div class="grid grid-cols-1 lg:grid-cols-3 gap-8">
      <!-- Colonne de gauche (adaptative sur mobiles et tablettes) -->
      <div class="lg:col-span-1 bg-slate-800 text-white rounded-lg shadow-2xl overflow-hidden">
        <div class="p-4 sm:p-6">
          <!-- Contenu de la colonne de gauche -->
          <div class="space-y-6">
            <!-- Première ligne : photo et contacts -->
            <div class="lg:grid-cols-1 sm:grid-cols-2 grid grid-cols-1 gap-6">
              <Photo class="w-full h-auto" />
              <Contacts />
            </div>
            <!-- Deuxième ligne : compétences, langues et loisirs -->
            <div class="grid grid-cols-1 lg:grid-cols-1 sm:grid-cols-2 gap-6">
              <Skills />
              <div class="space-y-6">
                <Languages />
                <Hobbies />
              </div>
            </div>
          </div>
        </div>
      </div>

      <!-- Colonne de droite -->
      <div class="lg:col-span-2 bg-white rounded-lg shadow-2xl overflow-hidden">
        <div class="p-4 sm:p-6 lg:p-8">
          <About class="mb-8" />
          <Projets class="mb-8" />
          <Experience class="mb-8" />
          <Education />
        </div>
      </div>
    </div>
  </div>
</template>

<style>
h1 {
  @apply font-bold text-gray-900 text-2xl md:text-3xl mb-4;
}
h3 {
  @apply font-bold text-gray-800 text-xl md:text-2xl mb-3;
}
i {
  @apply text-orange-500;
}
.bg-slate-800 h3 {
  @apply text-white;
}
</style>
