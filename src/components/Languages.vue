
<template>
    <!--language section-->
  <div class="soft-skills">
      <h3 class="sidebar-title">Language</h3>
      <ul class="list-disc pl-5">
          <li v-for="(language, index) in languages" :key="index" class="text-orange-500 p-1">
                 <span class="text-white">{{ language.name }} - {{ language.level }}</span>
          </li> 
      </ul>
  </div>
</template>

<script setup>
     const languages = [
        {
         name: 'Ukrainian',
         level: 'Native',
        },
        {
          name: 'Russian',
          level: 'Native',
        },
        {
          name: 'English',
          level: 'B1',
       },
        {
          name: 'French',
          level: 'B2',
        }
      ]
</script>