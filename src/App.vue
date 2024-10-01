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
  <div class="w-full grid grid-cols-3 px-32 py-7">
      <div id="aside" class=" bg-slate-800 text-white shadow-2xl">
        <Photo/>
          <div class="px-10 py-5">
            <Contacts/>
            <Skills/>
            <Hobbies/>
            <Languages/>
          </div>
      </div>
      <div class=" col-span-2 px-14 py-10 shadow-2xl">
        <About/>
        <Projets/>
        <Experience/>
        <Education/>
      </div>
  </div>
</template>

<style>
h1 {
 @apply font-bold text-black text-2xl;
}
h3 {
  @apply m-3 text-black font-bold text-2xl;
}
i {
  @apply text-orange-500;
}
#aside h3 {
@apply text-white;
}
</style>
