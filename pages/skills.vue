<template>
  <div>
    <div v-for="s in skills" :key="s.group" class="mb-6">
      <h2 class="font-semibold text-xl text-gray-900">
        {{ s.group }}
      </h2>
      <div class="flex flex-wrap">
        <p v-for="i in s.items" :key="i" class="text-justify pr-2">
          {{ i }}
        </p>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  data () {
    return {
      skills: [
        {
          group: 'Languages',
          items: ['JavaScript', 'Python', 'Java', 'HTML5/SCSS']
        },
        {
          group: 'Frameworks & Libraries',
          items: ['Node.js', 'Vue.js', 'Express.js', 'Quasar Framework', 'NestJS', 'Django', 'TailwindCSS', 'Bootstrap', 'scikit-learn', 'Keras']
        },
        {
          group: 'Tools',
          items: ['Git', 'Postman', 'PuTTY', 'Google Cloud Platform (Compute Engine)']
        },
        {
          group: 'Databases',
          items: ['MySQL', 'Firebase', 'SQLite']
        },
        {
          group: 'Others',
          items: ['Wordpress']
        }

      ]
    }
  }
})
</script>

<style>
</style>
