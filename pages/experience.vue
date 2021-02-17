<template>
  <div>
    <div v-for="e in experience" :key="e.name" class="mb-6">
      <h2 class="font-semibold text-xl text-gray-900">
        {{ e.name }}
      </h2>
      <p v-for="d in e.description" :key="d" class="text-justify">
        {{ d }}
      </p>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  data () {
    return {
      experience: [
        {
          name: 'Software Development Intern',
          description: [
            'Created a Python web scrapper using BeautifulSoup to retrieve details about leads and e-mail the results to a destination using the GMail API.',
            'Worked together with co-interns and professional developers to build an e-commerce API using Django and Django REST Framework.'
          ]
        },
        {
          name: 'Software Developer',
          description: [
            'Develops web applications using Node.js, Vue.js, Express.js, NestJS.',
            'Handles client concerns and coordinates with them on project requirements, scope, and contract terms in Chinese (Mandarin/Fokkien).']
        }
      ]
    }
  }
})
</script>

<style>
</style>
