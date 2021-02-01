<template>
  <div>
    <div v-for="p in projects" :key="p.name" class="mb-6">
      <h2 class="font-semibold text-xl text-gray-900">
        {{ p.name }}
      </h2>
      <p class="text-justify">
        {{ p.description }}
      </p>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
  data () {
    return {
      projects: [
        {
          name: 'ChromeExtensionKit',
          description: `I'm a motivated full-stack engineer who has experience building and
          scaling web applications and services in various domains. I'm also
          passionate about open-source contributions, working in high impact
          environments, and helping growing development teams build great
          products.`
        },
        {
          name: 'Lorem Ipsum Dolor',
          description: `Lorem ipsum dolor sit amet consectetur, adipisicing elit.
          Eius id eligendi reprehenderit, pariatur fugiat deleniti, omnis sequi
          soluta esse praesentium laborum obcaecati cumque, doloremque distinctio.`
        },
        {
          name: 'Lorem Ipsum Dolore',
          description: `Lorem ipsum dolor sit amet consectetur, adipisicing elit.
          Eius id eligendi reprehenderit, pariatur fugiat deleniti, omnis sequi
          soluta esse praesentium laborum obcaecati cumque, doloremque distinctio.`
        }
      ]
    }
  }
})
</script>

<style>
</style>
