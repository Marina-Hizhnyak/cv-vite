
<template>
  <!--my Education section-->
  <h3>Education</h3>
  <div class="mbg-gray-100 p-6 rounded-lg shadow-lg mb-6">
      <div v-for="(edu, index) in education" :key="index" class="p-2">
          <h4 class="text-lg font-bold text-orange-500">{{ edu.institution }}</h4>
          <h5 class="text-md italic text-gray-600">{{ edu.degree }}</h5>
          <p class="text-sm text-gray-500">{{ edu.location }} {{ edu.period }}</p>
      </div>
  </div>
</template>

  <script setup>
  const education = [
    {
      institution: 'Ifosup',
      degree: 'Web Development BES Training',
      location: 'Belgium',
      period: '2023 - 2025',
    },
    {
      institution: 'National Academy of Civil Engineering and Architecture of Donbass',
      degree: 'Business Economics',
      location: 'Ukraine',
      period: '2004 - 2009',
    },
  ];
  </script>