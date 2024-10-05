
<template>
    <!--hobbies section-->
  <div class="my-10">
      <h3 class="sidebar-title">Hobbies</h3>
      <ul class="hobbies-list">
          <li v-for="(hobby, index) in hobbies" :key="index" class="p-1">
                 <i :class="hobby.icon"></i>
                 <span class="pl-2">{{ hobby.name }}</span>
          </li> 
      </ul>
  </div>
</template>
<script setup>
     const hobbies = [
        {
         name: 'Reading',
         icon: 'ri-book-open-line',
        },
        {
          name: 'Roller-skating',
          icon: 'ri-golf-ball-line',
        },
        {
          name: 'Programming',
          icon: 'ri-reactjs-fill',
       },
        {
          name: 'Traveling',
          icon: 'ri-suitcase-3-line',
        }
      ]
</script>

