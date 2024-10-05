

<template>
    <!--my Work Experience section-->
    <h3>Work Experience</h3>
  <div class="bg-white shadow-md p-8 rounded-lg mb-8">
    <div v-for="(job, index) in workExperience" :key="index" class="job mb-4">
      <h4 class="text-lg font-semibold mb-2 text-orange-500">{{ job.position }} at {{ job.company }}</h4>
      <p class="text-sm text-gray-600 mb-4">{{ job.period }} <span class="mx-2">|</span> {{ job.location }}</p>
      <ul>
        <li class="list-disc list-inside" v-for="(duty, i) in job.duties" :key="i">{{ duty }}</li>
      </ul>
    </div>
  </div>
</template>


<script setup>
const workExperience = [
  {
    position: "Accountant",
    company: "Foxtrot - Gostomel",
    period: "September 2018 - April 2022",
    location: "Ukraine",
    duties: [
      "Managed financial records and ensured accuracy in accounting processes.",
      "Coordinated with other departments to ensure financial compliance and resolve issues.",
      "Developed and implemented efficient accounting procedures.",
      "Led a team of accountants and supervised daily accounting operations."
    ]
  },
  {
    position: "Online Store Manager",
    company: "Independent Company Koulikov",
    period: "January 2017 - August 2018",
    location: "Ukraine",
    duties: [
      "Managed online store operations, including inventory management and order processing.",
      "Developed marketing strategies to increase sales.",
      "Provided customer service and resolved product issues."
    ]
  },
  {
    position: "Credit Specialist",
    company: "OTP Bank",
    period: "June 2016 - January 2017",
    location: "Ukraine",
    duties: [
      "Evaluated credit applications and determined client eligibility.",
      "Advised clients on credit products.",
      "Managed credit files and tracked payments."
    ]
  }
]
</script>